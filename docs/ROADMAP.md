# Hoja de ruta

[Volver a la presentación](../README.md)

Estado revisado el **29 de octubre de 2026**. Las prioridades pueden cambiar durante el desarrollo; no se anuncian fechas de lanzamiento.

## Base integrada

- [x] Acceso compartido y permisos por espacio de trabajo.
- [x] Contactos, grupos y fichas con historial de relaciones.
- [x] Expedientes, personas vinculadas, notas y actuaciones.
- [x] Numeración anual común por despacho.
- [x] Documentos privados, versiones y organización Extrajudicial/Juzgado.
- [x] Agenda con recurrencias, excepciones y revisión personal.
- [x] Exportación de expedientes a ZIP con consulta legible.
- [x] Copias manuales, consulta histórica local, comparación y extracción de versiones.

Estas capacidades están incorporadas a la rama principal de desarrollo. La recuperación completa del sistema y la aceptación del piloto permanecen abiertas.

## Implementado en revisión

**Comunidades de propietarios.** Comunidad, inmuebles, propietarios y ocupantes, cotitularidad, historial, preferencias de notificación, reuniones y actas con versiones documentales. Incluye extensiones de exportación y consulta de copias.

La implementación está en una rama de revisión. La integración y la aceptación humana siguen pendientes. Registrar una preferencia de notificación no envía comunicaciones automáticamente.

## Ampliaciones previstas

| Área | Alcance previsto |
| --- | --- |
| Servicios y contratos | Proveedores, contratos, seguros y renovaciones vinculadas a agenda. |
| Incidencias y obras | Seguimiento de avisos, visitas, presupuestos y actuaciones relacionadas con reuniones. |
| Economía del despacho | Honorarios, provisiones, suplidos, cobros parciales y documentos de minutas. |
| Economía de comunidades | Ingresos, gastos, cuotas, justificantes y pendientes por inmueble y periodo. |
| Consulta global | Búsqueda transversal, pendientes y resúmenes imprimibles. |

El control económico previsto no anuncia emisión fiscal de facturas, integración bancaria ni interpretación automática de justificantes PDF.

## Consolidación antes del piloto

- [ ] Completar y verificar recuperación integral y recuperación tras perder o cambiar el equipo.
- [ ] Definir y validar el procedimiento autorizado de restauración remota.
- [ ] Revisar de forma integral sesiones, protección local, temporales y copias.
- [ ] Resolver incidencias de interacción y completar aceptación visual y funcional.
- [ ] Preparar instalador y actualización sin pérdida de información.
- [ ] Ensayar recorridos completos y recuperación en varios equipos Windows.

## Dirección futura: asistencia con IA

Se contempla incorporar ayuda para consultar información seleccionada, resumir documentación y preparar borradores sujetos a revisión humana.

Es una línea de exploración, todavía sin implementación. Antes de incorporarla habrá que concretar el alcance, los permisos sobre los documentos, el tratamiento de la información y los costes. No se anuncia automatización de decisiones jurídicas ni conexión de cuentas personales de ChatGPT.

## Plataformas

Windows es el objetivo actual. El uso de Flutter permite estudiar otras plataformas, pero macOS y móviles no tienen una versión anunciada ni una fecha comprometida.
