Aquí tienes un ejemplo de un `README.md` para el sistema de ajuste de FPS en Unity, sin incluir el código directamente:

---

# Sistema de Ajuste de FPS en Unity

Este proyecto permite al jugador seleccionar el límite máximo de FPS (fotogramas por segundo) a través de un `Dropdown`. Las opciones disponibles son: 24, 30, 60, 75, 120 y 144 FPS, con 144 siendo el máximo.

## Descripción

Este sistema proporciona una opción sencilla para que el jugador ajuste el límite de FPS a su preferencia. Las opciones disponibles en el `Dropdown` son:
- 24 FPS
- 30 FPS
- 60 FPS
- 75 FPS
- 120 FPS
- 144 FPS

El jugador podrá seleccionar cualquiera de estas opciones y el juego aplicará el cambio en tiempo real. Esto es útil para asegurar una experiencia optimizada según las capacidades del hardware del usuario.

## Requisitos

- **Unity 2020.3** o superior.
- Familiaridad con el sistema de UI de Unity, preferiblemente usando TextMeshPro (`TMP_Dropdown`).
- Opcional: Familiaridad con el sistema de `Dropdown` básico de Unity si prefieres no usar TextMeshPro.

## Uso

### Paso 1: Configurar el Dropdown

1. En tu escena de Unity, crea un objeto `Dropdown`:
   - **GameObject > UI > TextMeshPro - Dropdown**.

2. Asigna las opciones de FPS en el `Dropdown`. Las opciones deben ser: 24, 30, 60, 75, 120 y 144.

### Paso 2: Asignar el Script

1. Crea un `GameObject` vacío en la escena y nómbralo `FPSManager`.
2. Añade el script `FPSLimiter.cs` al `FPSManager`.
3. Arrastra el `TMP_Dropdown` desde la jerarquía al campo `fpsDropdown` en el Inspector del `FPSManager`.

### Paso 3: Ejecutar

Ejecuta el proyecto y selecciona la opción de FPS en el `Dropdown`. El límite de FPS se ajustará automáticamente según la opción seleccionada por el jugador.


## Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.
