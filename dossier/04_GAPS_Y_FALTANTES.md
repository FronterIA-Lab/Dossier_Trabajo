# Gaps y faltantes — lo que bloquea cobro o control

Organizado por tipo. Marca ✅ cuando lo cierres; no agregues filas nuevas sin borrar una.

---

## A. Bloquean cobro esta semana

| Faltante | Para qué | Dónde resolverlo |
|---|---|---|
| Link de pago (Stripe/Gumroad/PayPal/SPEI) | Curso / taller / libro | Landing Make-Taller + página A1 |
| Oferta publicada con precio visible | Que alguien pueda decir “sí” | Carrd / Notion / fronteria-lab.com |
| Demo 3 min reproducible | Vender B2B sin pitch abstracto | TEKTRON Jetson → video |
| SOW Diagnóstico Express (2 págs) | Anticipo A2 | Laboratorio / ops |
| SOW Piloto RAG Express (2 págs) | Anticipo B1 50% | Laboratorio / ops |
| Calendario de agenda (Cal.com u otro) | Agendar demos/taller | Sitio |
| CFDI + términos IVA verificados | Cobrar empresas MX | Contabilidad |
| NDA / política de datos plantilla | Cerrar legales/contables | 1 MD + PDF |

---

## B. Bloquean el curso digital (A3)

| Faltante | Nota |
|---|---|
| Videos/audios de lecciones | Lista en `Make-Taller-MCC/curso-digital-mcc/COMO-INSERTAR-MEDIA.md` |
| Media en `aula/media/` | Hoy solo `.gitkeep` |
| `modulos/` y `politica-de-uso.md` | Guía vendedor los menciona; existen en ZIP Archivo, no en árbol Make actual — sincronizar |
| Checkout en landing | Placeholder de precio sin link vivo |

**Atajo:** no grabar las 13 lecciones antes de vender. Publica **Módulo 1–2 + glifos + cuaderno** y entrega el resto por oleadas a compradores early.

---

## C. Bloquean libro

| Faltante | Prioridad |
|---|---|
| Canal de venta del PDF corregido | Alta |
| EPUB | Baja (después del primer cobro) |
| Limpieza de drafts en Libro-indioyori | Media (higiene mental, no venta) |

Canónica: `Archivo-final-MCC/libro/IndioYori-Teroyokori-Negro.pdf`.

---

## D. Bloquean instrumentos MACS / IPA como SKU

| Faltante | Nota |
|---|---|
| Precio lista Express / Completa publicado | Bitácora ya tiene zona; falta decidir y fijar |
| One-pager SOW MACS Express | Pedido en bitácora §3 |
| One-pager SOW IPA Express | Idem |
| Bloque en fronteria-lab.com | SKU separados (no “MACS/IPA”) |
| Bio actualizada | Viñetas separadas MCC / MACS / IPA |
| 1 piloto MACS | Corpus propio o aliado; no esperar a Antonio |
| Envío carta Senado | Borrador listo |

---

## E. Riesgos técnicos TEKTRON (no bloquean demo, sí bloquean escala)

| Gap | Severidad | Acción |
|---|---|---|
| Dual DIALECTICA 59.3% vs 60% | Baja para demo | Curar 1–2 preguntas corpus |
| Tag `TECNICO` nunca implementado | Media | No optimizar KPI equivocado; implementar o documentar defer |
| Sin snapshot post-L1 | Alta | Snapshot 3-2-1 ya |
| Git del sistema Jetson con 0 commits | Alta | Commit bridge L1 + README de arranque |
| `tektron_bridge.py` ≠ proceso vivo 7.0-l1 | Alta operativa | Documentar archivo canónico del proceso |
| Endpoints v6 (`/investigar`, `/calibrar-pdf`) ausentes | Baja | No son MVP de venta |
| hybrid-rag / industrial incompletos | N/A venta | Congelados |

---

## F. Gaps de control / organización (por eso estás “hecho bolas”)

| Gap | Efecto | Remedio |
|---|---|---|
| Misma obra en 3–5 repos | Editas la copia equivocada | Usar canónicas de `02_INVENTARIO_REPOS.md` |
| Bitácora vs plan ingresos desacoplados | Dos “verdades” de prioridad | Bitácora = ops diarias; Plan = dinero; este dossier = mapa |
| 20 temas blog + papers + 2 stubs código | Dilución | Regla: máx. 2 frentes |
| Research de ingresos ya cerrado pero se sigue “investigando” | Evitación de venta | Cerrar Laboratorio a solo checklist |
| Productos al 90% | Sensación de avance sin renta | Definir “hecho” = **alguien puede pagar** |

---

## G. Lo que NO te falta (deja de perseguirlo)

- Marco teórico sólido  
- Manual práctico  
- Método MCC documentado y con evidencia de campo  
- Instrumentos de auditoría e instrucción (MACS/IPA v1.0)  
- Demo técnica diferenciada (TEKTRON)  
- Investigación de mercado y precios  
- Outline y empaque de curso  
- Libro en PDF vendible  
- Keynote en guion  
- Red / beachhead pensado (medios → despachos → universidad)

Te falta **operación de cierre**: pago, demos, SOW, envíos, 20 nombres, anticipos.

---

## H. Checklist de higiene (1 tarde, cuando ya haya un cobro o envíos hechos)

- [ ] Elegir canónica por obra duplicada (tabla en `02_`)
- [ ] Mover o marcar drafts libro como `/archivo/`
- [ ] Verificar/eliminar `IA Poder y Autonomia Cognitiva_dup1.pdf`
- [ ] Sincronizar `politica-de-uso.md` ZIP → Make
- [ ] Actualizar README de cada repo con 1 línea de rol + link a este dossier
- [ ] Una sola Estrella Polar vigente (IndioYori vs TEKTRON — no mezclar docs)
