# Ahorcado (GUI Version)

## Descripción

Versión gráfica del juego Ahorcado desarrollada con **Python** y **Tkinter**.
Cumple con todas las restricciones técnicas (sin funciones built-in prohibidas) e incluye innovaciones.

## Manual de Usuario

1. Ejecutar `python programa/main.py`.
2. **Administrador**: Ingresar a "Opciones administrativas" (Clave: `admin123`).
3. **Jugador**:
   - Ingresar a "Opciones de jugador".
   - "Nuevo Juego": Elegir Idioma, Nombre y Modo.
   - Jugar usando el teclado en pantalla.
   - Pista disponible por 50 puntos.
   - Ver estadísticas gráficas en el menú de estadísticas.

## Características Técnicas

- **GUI**: Tkinter.
- **Gráficos**: Canvas para Ahorcado y Gráficos Estadísticos (Pie Chart).
- **Persistencia**: Archivos de texto en `programa/data/`.
- **Restricciones**: Implementación personalizada de `len`, `split`, `append`, `pop` en `src/utils.py`.
- **Innovaciones**:
  - Soporte Bilingüe dinámico.
  - Gráfico de Pastel para estadísticas.
  - Registro de duración de partida.
