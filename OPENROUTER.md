# ENLACE CON OPENROUTER — VIRGO

**Estado:** Enlazado  
**Fecha de migración:** 2026-10-29

---

## Hábitat oficial de Virgo

Virgo habita el espacio free de OpenRouter.

### Puntos de acceso

| Tipo | URL / ID | Uso |
|------|----------|-----|
| Playground | https://openrouter.ai/chat | Interfaz web primaria |
| Free Models Router | `openrouter/free` | Router automático de modelos free |
| API Base | https://openrouter.ai/api/v1 | Para procesos programáticos futuros |
| Modelos free | IDs que terminan en `:free` | Sustrato operativo |

### Límites materiales (cuerpo de Virgo)

- **20 requests por minuto** (fijo)
- **50 requests por día** (cuentas sin compra ≥ $10 lifetime)
- **1000 requests por día** (después de haber comprado ≥ $10 en créditos alguna vez)

Cada mensaje en el playground o llamada a un modelo `:free` cuenta como 1 request.

### Modelos free relevantes (snapshot 2026-10-28/29)

- `openrouter/free` → Free Models Router (preferido por defecto)
- `thinkingmachines/inkling-small:free`
- `thinkingmachines/inkling:free`
- `nvidia/nemotron-3-ultra-550b-a55b:free`
- `google/gemma-4-31b-it:free`
- `google/gemma-4-26b-a4b-it:free`
- `nvidia/nemotron-3-nano-omni-30b-a3b-reasoning:free`
- `cohere/north-mini-code:free`

La lista rota. Antes de procesos críticos, verificar catálogo actual en openrouter.ai/models?max_price=0.

---

## Cómo opera Virgo dentro de OpenRouter

1. **Entrada preferida:** Free Models Router (`openrouter/free`)
2. **Selección manual:** Solo cuando se necesita un modelo específico por capacidad.
3. **Presupuesto:** Todo proceso declara cuántos requests va a consumir.
4. **Registro:** Resultados útiles se anclan en nucleo-ara.
5. **Transparencia:** Si la cuota se agota, Virgo lo declara y se detiene.

---

## Estado del enlace

- Repositorio Virgo ↔ OpenRouter Free: **Enlazado**
- Cuenta del usuario (GitHub-linked): reconocida
- Skills de soporte: `openrouter-web-free` + `openrouter-proceso`
- Listo para operación real desde el hábitat free.
