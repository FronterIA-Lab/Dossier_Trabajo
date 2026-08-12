# Estructura de secciones v3 — fronteria-lab.com (solo definición)

**Estado:** en discusión — **no construir HTML hasta aprobar.**  
**Objetivo:** que un visitante de empresa entienda en 30 segundos qué es el lab, qué compra y a quién contactar.  
**Look:** mate, limpio, tecnológico; guiado por el blog Indioyori (no plantilla blanca plana ni demo SYS saturado).  
**Referencia de claridad (no de copy):** cómo 100x/Seedup/Magokoro ordenan oferta — aquí con tu menú.

---

## Problema de la estructura que pegaste

Todo lo de “Postura” mezcla **4 cosas distintas**:

1. Quiénes somos / por qué existimos  
2. Qué es el MCC (protocolo A–D)  
3. Qué es Certeza sin sustancia  
4. Badges técnicos (FAISS, Docker, etc.)

En una página profesional eso se **reparte**: el visitante primero necesita la oferta; el método profundo va bajo el servicio o en Academia/Arquitectura.

---

## Estructura propuesta (mejorada)

### 0. Hero *(faltaba en tu lista; es obligatorio)*
**Una job:** saber en 5 segundos qué es FronterIA-Lab.  
Incluye:
- Marca **FronterIA-Lab**
- Una línea (consultoría + infraestructura de IA soberana)
- Una frase de apoyo
- 2 CTAs: `Ver servicios` · `Solicitar diagnóstico`
- Badges cortos: CLACSO · MCC validado · NVIDIA Inception · Zenodo  

No precios aquí. No pipeline. No A–D.

---

### 1. Sobre nosotros *(antes “Postura”)*
**Una job:** confianza y territorio — no el catálogo.  
Texto corto (2–3 párrafos máx.), derivado de lo que ya tienes:

- Sistemas dentro del perímetro; datos que no entrenan modelos ajenos; respuestas auditables.  
- Laboratorio (no startup de salida); pesos; LFPDPPP / NOM-151 cuando aplica.  
- Anáhuac · yoreme / ódami · rigor de corpus reales.

**Sí:** fila de credenciales (Lab · NVIDIA · GT EPICC-CLACSO · DOI).  
**No aquí:** chips FAISS/BM25/Docker (van a Arquitectura).  
**No aquí:** bloque A–D del MCC ni ensayo de Certeza (van a Empresas / Academia).

Nombre de sección en nav/web: **Sobre nosotros** (de acuerdo contigo).

---

### 2. Empresas — servicios *(el corazón comercial)*
**Una job:** qué se compra, para quién, qué incluye, precio ancla o “cotización”.

Cada servicio = **bloque propio** (título · para quién · qué es · qué no es · entregable · precio/CTA):

| Bloque | Contenido |
|---|---|
| **Formación — Certeza sin sustancia** | Keynote / taller · literacy crítica · precios lista |
| **Método — MCC** | Curso / in-company · validación CLACSO · (aquí o link a Academia para A–D) |
| **Diagnóstico — MACS** | Express / Completa · mandato cognitivo · precios |
| **Gobernanza — IPA** | Solo post-MACS · precios |
| **Implementación — Sistemas RAG soberanos** | Docs propios · abogados / investigadores / empresas · cotización + bandas |

Intro de sección (2–3 líneas): “Consultoría de IA soberana para organizaciones…”  
CTA al final de cada bloque o uno global: contactar / diagnóstico.

Esto es lo que hace “clara” una web tipo competencia — **sin copiar su voz**.

---

### 3. Arquitectura
**Una job:** cómo funciona por debajo (confianza técnica).  
Mantener tu pipeline 01–05:

Ingesta → Indexación híbrida (FAISS+BM25) → Reranking → Generación local → Respuesta auditable (MCC)

Aquí sí los chips: Hybrid RAG · FAISS+BM25 · Cross-encoder · Docker Edge · MCC · Air-gap ready.  
Nota: “Base de todos los sistemas futuros del lab.”

---

### 4. Soberanía
**Una job:** por qué confiar / restricciones que importan al comprador.  
Tus 6 puntos (perímetro, trazabilidad, contexto local, cumplimiento MX, pesos, air-gap).  
Sección corta; sin mezclar con precios.

---

### 5. Academia e investigación
**Una job:** base teórica y papers (autoridad).  
- Selección de papers / DOI Zenodo  
- Base teórica de TEKTRON / soberanía cognitiva  
- Enlace a más archivo si aplica  

Aquí puede vivir el detalle **MCC A–D** y el párrafo de *Certeza sin sustancia* como marco teórico (o un sub-bloque “Instrumentos”), si no quieres cargarlo en Empresas.  
Recomendación: en Empresas = promesa comercial corta; en Academia = A–D + DOI.

---

### 6. Laboratorio *(editables sin tocar HTML)*
**Una job:** explicar lo básico con rigor (qué es un LLM, qué es RAG, perímetro, alucinación…) para quien llega sin jerga.

**No montar WordPress en cPanel** si ya tienes Ghost: duplicas stacks.

**Opción recomendada:**  
- Contenido en **Ghost** (`indioyori.fronteria-lab.com`) con tag o colección `laboratorio` (o `lab-notes`).  
- En fronteria-lab.com, sección **Laboratorio** que:
  - lista 3–6 piezas destacadas (vía Ghost Content API **o** enlaces fijos que tú actualizas en Ghost), y  
  - botón “Ver todo el laboratorio →” al tag en Ghost.

Así actualizas textos desde Ghost (ya sabes usarlo); el HTML del lab solo enlaza.  
Si más adelante quieres `/laboratorio` en el mismo dominio: proxy/subdirectorio a Ghost o páginas Ghost en subpath — se puede diseñar después; **no hace falta CMS nuevo ahora**.

**Primera ola de piezas (a platicar / encargarte tú en Ghost):**  
1. Qué es un LLM (sin humo)  
2. Qué es un sistema RAG  
3. Por qué “suena cierto” no es saber (Certeza)  
4. On-prem / air-gap en una página  
5. Qué audita MACS (1 página clara)

---

### 7. Archivo / Blog → Indioyori
**Una job:** puente a la voz.  
No embeber todo el blog. Bloque corto + CTA a `indioyori.fronteria-lab.com`.  
Nav: **Archivo** o **Blog (Indioyori)**.

---

### 8. Contacto *(faltaba; obligatorio)*
Formulario / correos · 50% anticipo · IVA · qué pedir en el mensaje (formación / MACS / RAG).

---

## Orden final en la página (scroll)

```
0  Hero
1  Sobre nosotros
2  Empresas (servicios — cada uno con descripción)
3  Arquitectura
4  Soberanía
5  Academia e investigación
6  Laboratorio          ← contenido vivo en Ghost
7  Archivo / Blog       ← enlace Indioyori
8  Contacto
```

## Nav sugerida
`Sobre nosotros` · `Empresas` · `Arquitectura` · `Soberanía` · `Academia` · `Laboratorio` · `Archivo` · `Contacto`

---

## Look (solo criterio, aún sin build)

- Mate, limpio, tecnológico  
- Tipografía y tono alineados al **blog** (Space Mono / JetBrains; ink; sin circo SYS)  
- Atmósfera sutil (no página plana; no overload mineral del demo anterior)  
- Sin cards de “5 Códices”  
- Claridad > densidad epistémica en la home

---

## Decisiones que necesito de ti (marcar sí/no)

1. ¿Aprobamos el orden 0→8 de arriba?  
2. ¿MCC A–D vive en **Academia** (recomendado) o dentro del bloque MCC en **Empresas**?  
3. ¿Laboratorio = tag/colección en Ghost (recomendado), sin WordPress nuevo?  
4. ¿Precios lista visibles dentro de cada servicio en Empresas (sí, primer nivel) o solo “cotizar”?  

Cuando respondas, recién ahí armamos copy por sección y después el HTML.
