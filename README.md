# 🪝 Godot 4 — 3D Grappling Hook & Winch Physics System

Addon completo y personalizable de **Gancho de Agarre 3D y Cabrestante (Winch)** para **Godot 4**, con soporte para personajes en primera/tercera persona y extensión para vehículos pesados / grúas de rescate (`VehicleBody3D`).

---

## 🌟 Características Principales

- **Nodo `HookController` para Personajes (`CharacterBody3D`)**:
  - Lanzamiento rápido de gancho con detección de puntos de anclaje mediante raycasting.
  - Tensión de cable elástica / rígida basada en resortes físicos (Spring Physics).
  - Retracción y balanceo pendular natural en 3D.
- **Extensión para Vehículos y Grúas (`VehicleBody3D`)**:
  - Integración en `vehicle_body_3d.gd` para anclar ganchos desde la punta de una pluma de grúa (`Marker3D`).
  - Activación/desactivación dinámica de gancho al subir y bajar de vehículos mediante áreas de detección (`Area3D`).
- **Plataformas y Obstáculos Móviles**:
  - Script `rigid_body_3d_4.gd` y `moving_box.gd` para anclaje a elementos cinemáticos y móviles.

---

## 📂 Estructura del Proyecto

```text
godot-grappling-hook-3d/
├── addons/
│   └── grappling_hook_3d/
│       ├── src/                 # Código fuente del plugin de gancho
│       └── example/             # Escena de demostración
│           ├── vehicle_body_3d.gd   # Integración con grúa / vehículo
│           ├── rigid_body_3d_4.gd   # Cuerpos móviles de prueba
│           ├── player.gd            # Controlador del jugador
│           └── main.tscn            # Nivel de pruebas 3D
├── media/                       # Iconos y recursos visuales
├── project.godot                # Configuración de Godot 4
├── README.md                    # Documentación
└── ROADMAP.md                   # Hoja de ruta técnica
```

---

## 🚀 Requisitos y Uso

1. **Versión de Godot**: Godot Engine 4.0 o superior (compatible con Godot 4.2+ / 4.3+ / 4.5+).
2. **Ejecución**:
   - Abre Godot y carga el proyecto.
   - Ejecuta la escena `addons/grappling_hook_3d/example/main.tscn` (`F5`).
   - Usa el botón izquierdo del ratón para engancharte a superficies y la barra espaciadora para soltar.

---

## 📄 Licencia

Código abierto bajo licencia MIT. Consulta [LICENSE.md](LICENSE.md).
