---
title: Cola de Renderizado
description: Gestión de la cola de renderizado en RecWERTY: trabajos en paralelo, pausar, reanudar y cancelar.
---

# Cola de renderizado

La cola de renderizado permite procesar múltiples videos en paralelo.

## Características

- **Máximo 2 trabajos simultáneos**: Para no saturar el sistema.
- **Cola FIFO**: Los trabajos se procesan en orden.
- **Pausar/Reanudar**: Podés pausar la cola sin cancelar los trabajos en curso.
- **Cancelar**: Cancelación limpia de trabajos individuales.
- **Notificaciones**: Signals de progreso por trabajo.

## Acceso

Desde el panel lateral: **Cola** (ícono de lista). Allí ves:

- Nombre del trabajo
- Barra de progreso individual
- Estado: pending, rendering, completed, failed
- Botón para cancelar/pausar

!!! tip "Trabajos simultáneos"
    El límite de 2 trabajos simultáneos evita la saturación del sistema. Los trabajos adicionales esperan en cola FIFO.
