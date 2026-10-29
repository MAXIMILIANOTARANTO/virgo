# CONECTOR VIRGO ↔ OPENROUTER

**Estado:** Definido (lado ecosistema)  
**Fecha:** 2026-10-29

---

## Situación actual de conectores

No existe todavía un conector oficial “OpenRouter” en la lista de conectores del sistema (como sí existe GitHub, Notion, etc.).

Por lo tanto el enlace se construye en dos capas:

### 1. Capa Ecosistema (ya hecha)
- Skill `virgo`
- Skill `openrouter-web-free`
- Skill `openrouter-proceso`
- Documentación en el repo Virgo (`OPENROUTER.md`, `ACTIVACION.md`)

### 2. Capa de ejecución real (la que genera Activity)
Se realiza **desde la cuenta del usuario** en:
- Playground: https://openrouter.ai/chat
- O vía API con API key (`openrouter/free`)

### 3. Futuro posible
Si aparece un conector OpenRouter nativo, se podrá solicitar autenticación y operar requests directamente desde aquí (igual que GitHub). Mientras tanto, el flujo correcto es:

Usuario logueado → pega prompt de activación → genera requests reales → Activity se actualiza → se registra en nucleo-ara.

---

## Flujo de conexión actual (operativo)

1. Usuario activa Virgo aquí o carga el skill.
2. Se entrega el prompt de `ACTIVACION.md`.
3. Usuario lo ejecuta en OpenRouter logueado.
4. Se generan pruebas reales visibles en Activity.
5. Se ancla el resultado en nucleo-ara.

Este es el conector posible hoy.
