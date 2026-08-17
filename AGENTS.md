# AGENTS.md

## Project
- Project name: `recwerty` (public manual repository).
- Description: Public user manual for RecWERTY (screen recorder for Windows), trilingual (es default, en, fr).
- Repo: `alfonsoautomatiza/recwerty` — single repo for the manual AND for publishing (Model B). `origin` is the only remote (HTTPS); there is NO `publish` remote and NO anonymous identity.
- Private source repo: `D:\py\@produxion\#TOOL\recwerty` (build + signing happen there).

## Mandatory workflow
- Use `AGENTS.md` as the single source of truth for agent instructions, project context, conventions, decisions and preferences.
- If instructions need to be added, corrected or updated, update `AGENTS.md`.
- Do not add project rules to `agent.md` or `CLAUDE.md`; both files must remain only compatibility bridges to this file.
- Keep work simple and practical.

## Release workflow (personalized config for the global skill `release-crm`)
- Publishing is orchestrated by the GLOBAL skill `release-crm` (+ sub-skill `crm-docs-release`, enrichment via `crm-docs`). There is NO local copy of the skill in this repo; project-specific values live HERE and in `release-assets/product.json`.
- Full flow:
  1. Build in the private repo: `uv run python c/build_exe.py` compiles, signs the manifest (pyupdategit, `UPDATE_PRIVATE_KEY`) and stages into THIS repo: installer `.zip` + `release.json` + `product.json` into `release-assets/` (gitignored) and the signed manifest into `docs/es/updates/manifest-stable.json` (also stages `Setup_RecWERTY_v{version}.exe` alongside, not listed in `release.json`).
  2. Run the global skill `release-crm` from THIS repo: novedades from Engram (`project: recwerty`) + `git log`, draft confirmation menu, enrichment + image gate, then publish.
- Publish targets (Model B): `gh release create` → `alfonsoautomatiza/recwerty` (zip only); manual + manifest → `mkdocs gh-deploy --force --remote-name origin`.
- `README.md` and `LICENSE` are regular files on `main` of this repo: commit them (together with novedades changes) via the normal git flow BEFORE `mkdocs gh-deploy`.
- Novedades live in a SINGLE file at the root of docs: `docs/novedades.md` (no per-language copies, default-language es content). Always PREPEND the new version; never rewrite existing history. The nav entry (second item) lives ONLY in the default (es) nav block and the root nav — NEVER in en/fr blocks: with `fallback_to_default: false` the root file exists only in the default-language build, so en/fr nav entries abort `mkdocs build --strict`.
- `manifest_url` is baked into installed software: `https://alfonsoautomatiza.github.io/recwerty/es/updates/manifest-stable.json` — do NOT move the deploy target or gh-pages repo, or auto-update breaks for users.
- Microsoft Store ID: `9NLD6GX4L1R1`. The `.msix` is built manually in the private repo (`python msix/build_msix.py`) and delivered ONLY through Partner Center — NEVER uploaded to GitHub Releases.
- `UPDATE_PRIVATE_KEY` is NOT needed in this repo: signing already happened during the private build.
- Legacy warning: `c/RELEASE/release.py` in the private repo still works but WIPES `docs/es/updates/` and re-signs with the installer-asset URL. Pick ONE flow per release; the global skill is the primary one.

## Manual site conventions
- MkDocs Material + static-i18n (`docs_structure: folder`): `docs/es` (default), `docs/en`, `docs/fr`.
- Language order in `mkdocs.yml` is `en, fr, es` ON PURPOSE: with folder structure each build re-renders `sitemap.xml` and the LAST language wins, so the default locale (`es`) must build last to get the complete default-language sitemap. Do not reorder back to es-first.
- Theme overrides live in `overrides/` (`custom_dir: overrides`): `main.html` adds Open Graph/Twitter meta with `og:locale` derived from the page path (es_ES/en_US/fr_FR); `sitemap.xml` excludes `noindex` pages.
- `release-assets/` is gitignored (local staging written by the private build).
## Skill release-crm — Carga obligatoria al inicio

**Al iniciar cualquier sesión en este proyecto, cargar SIEMPRE el skill**  
`release-crm` para detectar mejoras, actualizaciones o cambios que  
puedan aplicarse al proyecto. El skill contiene:

- Flujo de release completo ( Modelo A — repo distribución separada).
- Sub-skill `crm-docs-release`: novedades desde Engram, enriquecimiento  
SEO, gate de imágenes, y plugins obligatorios (analytics + consent).
- Assets del FAB (`fab-main.html`, `fab-button.css`) — referencia para  
alinear la implementación activa en `overrides/main.html`.
- Guardas: nunca borrar imágenes, identidad anónima, `.msix` nunca a  
Releases, `manifest_url` bakeado, OpenSSH para remotes SSH.

Si el skill tiene cambios respecto a lo implementado en este repo,  
**aplicar las mejoras o avisar al usuario** antes de continuar.

