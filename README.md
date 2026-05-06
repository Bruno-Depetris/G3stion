# G3stion - Documentación del Proyecto

Documentación completa del proyecto G3stion, organizada en cuatro documentos según su propósito.

## Índice

| Documento | Propósito | Audiencia |
|-----------|-----------|-----------|
| [Vision.md](./Vision.md) | El **por qué** del proyecto. Problema, propuesta de valor, usuario objetivo, modelo de negocio, criterios de éxito. | Todos. Empezar por acá. |
| [Product-Spec.md](./Product-Spec.md) | El **qué** funcional. Alcance del MVP, historias de usuario, reglas de negocio, flujos, UI/UX. | Producto + desarrollo. |
| [Technical-Spec.md](./Technical-Spec.md) | El **cómo** técnico. Stack, arquitectura, modelo de datos, API, seguridad, despliegue. | Desarrollo. |
| [Roadmap.md](./Roadmap.md) | El **cuándo**. Fases, estimaciones, cronograma, plan de contingencia. | Todos. |

## Resumen ejecutivo

**G3stion** es una aplicación SaaS multi-tenant orientada a emprendedores argentinos que venden productos físicos por Instagram, para reemplazar el control en Excel/papel.

- **Stack**: Blazor PWA + ASP.NET Core 9 + PostgreSQL 16 + Railway.
- **Arquitectura**: Clean Architecture + multi-tenancy con `tenant_id` y Row-Level Security.
- **Equipo**: 1 líder técnico (junior, 5 hs/semana) + 3 colaboradores ocasionales.
- **MVP estimado**: 6 a 9 meses desde el inicio.
- **Validación**: 4 usuarios reales esperando.
- **Modelo**: pago obligatorio post-validación, ARS $10.000/mes objetivo.

## Decisiones pendientes (bloquean el inicio)

1. **Idioma de BD**: inglés (recomendado) vs español.
2. **Nombre del producto**: G3stion vs Predits (el dominio existente).
3. **Roles del equipo**: definir qué hace cada colaborador.
4. **Día de sync semanal**: para el check-in de 30 min.

## Cómo usar esta documentación

- **Si sos nuevo en el proyecto**: leé en este orden → Vision → Product-Spec → Technical-Spec → Roadmap.
- **Si venís a desarrollar una HU**: andá a Product-Spec (ver historia y criterios) y Technical-Spec (ver modelo de datos y endpoints).
- **Si querés saber el estado del proyecto**: andá a Roadmap.
- **Si tenés dudas sobre una decisión**: buscá en Technical-Spec sección "Decisiones técnicas justificadas".

## Mantenimiento de la documentación

- Estos documentos son **vivientes**. Se actualizan a medida que el proyecto evoluciona.
- Cualquier cambio importante en el alcance, stack o arquitectura debe reflejarse acá **antes** de implementarse.
- Cada documento tiene un campo "Versión" y "Última actualización" en el header. Mantenerlo al día.
- El proceso para cambiar algo: PR a la rama `main` con la modificación, descripción clara del cambio.

---

> **Nota**: el archivo original `excerpt_from_previous_claude_message.txt` queda como referencia histórica del primer borrador. Todos los documentos en esta carpeta lo reemplazan y refinan.
