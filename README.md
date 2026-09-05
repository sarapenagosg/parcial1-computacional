# Parcial 1 — Sistemas Inteligentes II + Introducción al Deep Learning

**Estudiante:** Sara Penagos
**Curso:** Sistemas Inteligentes II + Introducción al Deep Learning
**Periodo:** 2026-2

## Contenido del repositorio

- `computacional/Perceptron_Rosenblatt_parcial1.ipynb`: implementación del perceptrón
  de Rosenblatt (funciones elementales, funciones coordinadoras, experimentos con
  AND, XOR y datos sintéticos).
- `computacional/ADALINE_parcial1.ipynb`: implementación de ADALINE con arquitectura
  funcional propuesta, entrenada mediante batch gradient descent.
- `teorico/pacial1si_teorico.pdf`: entrega de la parte teórica del parcial.
- `src/parcialsi1/`: estructura base del paquete generada por `uv`.
- `pyproject.toml` / `uv.lock`: definición y bloqueo de dependencias del proyecto.

## Instalación

Este proyecto usa [uv](https://docs.astral.sh/uv/) para gestionar dependencias.

```bash
uv sync
```

## Ejecución de pruebas

```bash
uv run pytest
```

## Revisión de estilo

```bash
uv run ruff check .
```

## Ejecutar los cuadernos

Abrir en VS Code y seleccionar como intérprete el ambiente creado por `uv`
(carpeta `.venv` dentro del proyecto), luego ejecutar **Restart Kernel → Run All**
en cada notebook dentro de `computacional/`.

## Observaciones

- Los dos cuadernos son autocontenidos: generan sus propios datos sintéticos
  internamente, no requieren archivos externos adicionales.
- `ADALINE_parcial1.ipynb` no usa `early stopping`: siempre ejecuta el número
  completo de épocas indicado.
