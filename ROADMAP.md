# 🗺️ Hoja de Ruta (Roadmap) — Godot 3D Grappling Hook

Este documento define la trayectoria técnica para la expansión del sistema de ganchos, cuerdas físicas y cabrestantes en Godot 4.

---

## 📌 Fase 1: Mecánica de Gancho y Soporte para Vehículos (Completado ✅)
- [x] Controlador modular de gancho para personajes `CharacterBody3D`.
- [x] Extensión para grúas y vehículos pesados (`VehicleBody3D`).
- [x] Anclaje a objetos rígidos en movimiento (`RigidBody3D`).
- [x] Limpieza de caché `.godot` y archivos temporales `.tmp`.

---

## 📌 Fase 2: Simulación de Cuerda Dinámica con Nodos Verlet (En Progreso 🔄)
- [ ] **Renderizado de Cuerda Catena / Verlet 3D**:
  - Reemplazo de línea recta por simulación de cable segmentado con peso, combadura (*sagging*) y colisión con bordes.
- [ ] **Sistema de Cabrestante de Recuperación (Winch)**:
  - Arrastre progresivo de vehículos pesados atascados en barro o nieve.
  - Limitador de tensión máxima antes de rotura de cable (*snap tension*).
- [ ] **Múltiples Puntos de Anclaje Simultáneos**:
  - Soporte para cables de estabilización y tirantes de carga para grúas.

---

## 📌 Fase 3: Audio Procedural y Polish Visual 🚀
- [ ] **Efectos de Partículas en Impacto**:
  - Chispas en superficies metálicas y fragmentos de roca en concreto.
- [ ] **Audio Reactivo a la Tensión**:
  - Sonido metálico creciente al acercarse al límite elástico del cable.
