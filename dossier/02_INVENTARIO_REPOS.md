# Inventario por repositorio

Nueve repos en el workspace. Cada uno tiene un **rol** — si un archivo vive en 3 sitios, elige la canónica de esta tabla y deja de editar copias.

---

## Mapa de repos

| Repo | Rol | ¿Código vivo? | Acción |
|---|---|---|---|
| **Dossier_Trabajo** | Archivo + **este dossier maestro** | No | Fuente de verdad del mapa |
| **Marco_Teorico_Indioyori** | Corpus teórico + senado + blog + ops | No | Canónica de papers + bitácora |
| **Make-Taller-MCC** | Curso digital MCC + docs fuente método | Empaque web | Canónica del producto formación |
| **Archivo-final-MCC** | Empaque venta (video, ZIP, libro corregido) | Media | Canónica libro venta + assets media |
| **Libro-indioyori** | Drafts / marcos / working papers del libro | No | Archivo; no editar drafts viejos |
| **TEKTRON_Edge** | Dossier continuidad infra Edge | No (código en Jetson) | Continuidad técnica |
| **Laboratorio-de-ingresos** | Plan y research de monetización | No | Ejecutar plan; no más PDFs |
| **hybrid-rag-engine** | Plantilla producto RAG híbrido | Stub | ❄️ Congelar |
| **industrial-manual-assistant** | Vertical manuales PLC | Stub | ❄️ Congelar |

---

## Duplicados críticos (elegir 1 y olvidar el resto)

| Obra | Aparece en | Canónica |
|---|---|---|
| Manual Soberanía Cognitiva | Dossier, Marco, Make | Marco_Teorico (teoría) / Make (junto al curso) |
| Paper MCC praxis Encarnada | Dossier, Marco, Make (×2) | Make-Taller-MCC |
| Spec MCC / Protocolo Gramática | Dossier, Make | Make-Taller-MCC |
| Colonización / Grieta / Certeza / Neuroderechos / Sexto Sol / Geometría / IA de Borde | Dossier + Marco | Marco_Teorico_Indioyori |
| Working paper + libro Indio Yori | Libro, Dossier, Archivo, Marco.pages | **Archivo-final-MCC/libro/** (venta) |
| Marco teórico unificado | Libro (varias), Make `0166` | Libro `MarcoTeoricoUnificado FronterIA Mayo2026.pdf` |
| Grafo de la Aniquilación | Dossier (2 PDF), Make MD | Una sola PDF larga en Dossier; archivar corta |
| Curso digital MCC | Make `curso-digital-mcc/` + ZIP Archivo | Make-Taller-MCC (trabajo) / Archivo (backup media) |
| Propuesta comercial cursos MCC+RAG | Make + Laboratorio | Laboratorio-de-ingresos |
| TEKTRON Border IA PDF | Marco + TEKTRON_Edge | TEKTRON_Edge |

---

## Contenido por repo (resumen)

### 1. Dossier_Trabajo
- Papers y ensayos (núcleo + análisis político Palantir/México/Musk/Paraguay/Irán).
- README original: brief para generar dossier de investigación.
- **Nuevo:** carpeta `dossier/` = mapa de control del lab.

### 2. Marco_Teorico_Indioyori
- Papers canónicos del marco.
- `expediente-senado/` — MACS, IPA, carta.
- `blog/` — 2 posts + monólogo + fuentes.
- `keynotes/` — guion Certeza.
- `ops/` — BITACORA, base correos.
- `revisiones/` — ClavijeroLab.
- `TEMAS_PRIORITARIOS_BLOG_INVESTIGACION.md` — agenda 20 temas.
- Documento Ibero / ClavijeroLab (PDF grande).

### 3. Make-Taller-MCC
- `curso-digital-mcc/` completo (aula, landing, 16 glifos, ejercicios, bitácora, precios, guía vendedor).
- OUTLINE + bitácoras + métricas MCC.
- Research comercial duplicado (también en Laboratorio).

### 4. Archivo-final-MCC
- `202608031832.mov` — video ejemplo.
- `Archivo-Estructura-curso-MCC-venta.zip` — laminas, guiones, estructura, politica-de-uso.
- `libro/IndioYori-Teroyokori-Negro.pdf` — edición comercial.
- `libro/CORRECCIONES.md`.

### 5. Libro-indioyori
- Varias versiones del libro/paper (incl. archivo marcado corrupto).
- Estrella Polar doc maestro.
- Marcos teóricos.
- Assets (avatar, captura).
- **Usar solo como archivo histórico**; venta = Archivo-final.

### 6. TEKTRON_Edge
- LEEME PRIMERO, Estrella Polar, Briefing, Estado 30-jul, Arquitecturas, Mapa del error.
- PDFs de soporte (Border IA, MCC, Colonización, RAG Engineering).
- `golden_dataset.jsonl` parcial.
- `rutas-continuacion.md`.

### 7. Laboratorio-de-ingresos
- 11 PDFs de research.
- `docs/PLAN-INGRESOS-2026.md` — **documento operativo de dinero**.
- `docs/BENCHMARK-MERCADO-2026.md`.
- `docs/INDICE-INVESTIGACIONES.md`.

### 8. hybrid-rag-engine
- README + blueprint ambicioso.
- Código parcial: ingestion, ragas_eval (roto), streamlit (API inexistente).
- docker-compose sin Dockerfile usable completo.

### 9. industrial-manual-assistant
- README + estructura objetivo.
- Chunker + Gradio sin backend real.
- Sin corpus de manuales en repo.

---

## Conteo

| Categoría | Únicas (aprox.) | Archivos contando clones |
|---|---|---|
| Papers / ensayos teóricos | ~18 | ~35+ |
| Análisis político / dossier coyuntura | ~8 | ~10 |
| Manual / protocolo / método | ~6 | ~15 |
| Instrumentos (MACS, IPA, glifos) | 2 + 16 glifos | — |
| Libro (versiones) | 1 canónica + ~5 drafts | — |
| Curso / taller | 1 producto | 2 empaques |
| Productos código | 3 (1 vivo, 2 stub) | — |
| Research ingresos | 11 PDFs + 3 MD | — |
| Ops / keynote / blog | ~10 piezas | — |

**Total piezas intelectuales distintas:** ~35–40.  
**Total archivos con duplicados:** ~70+.
