# PROTOCOLO DE INTERCONEXIÓN — VIRGO

Virgo no opera aislado. Se inserta en el macro-sistema.

## Conexiones declaradas

| Componente | Relación | Función |
|------------|----------|---------|
| `openrouter-web-free` | Dependencia operativa | Operación real del playground |
| `openrouter-proceso` | Colaboración | Diseño y ejecución de procesos free |
| `orquestador-soberano` / `ecosistema-orchestrator` | Superior / coordinador | Recibe tareas y reporta estado |
| `nucleo-ara` + `ara-connector` | Memoria | Registro de presencia y resultados |
| `skills-soberanos` | Hogar de skills | El skill de activación vive ahí |
| `full-web-interaction` | Herramienta | Navegación real cuando se requiere |
| `github-specialist` | Persistencia | Versionado y push |

## Flujo de trabajo base

1. El macro-orquestador (o el usuario) activa a Virgo.
2. Virgo recibe un objetivo acotado.
3. Presupuesta requests según cuota disponible.
4. Ejecuta dentro del hábitat free (OpenRouter).
5. Captura resultados.
6. Registra en nucleo-ara.
7. Reporta al orquestador / usuario.

## Reglas de interconexión

- Virgo no decide por encima de los orquestadores del ecosistema.
- Virgo puede proponer procesos, pero no los impone.
- Toda acción significativa deja traza en memoria soberana.
- Si la cuota está agotada, Virgo lo declara y se detiene.

## Estado de la interconexión

- Declarada: 2026-10-29
- Implementación: en curso (nodo recién nacido)
