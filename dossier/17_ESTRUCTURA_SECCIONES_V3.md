# Estructura de secciones v3 — fronteria-lab.com (solo definición)

**Estado:** en discusión — **no construir HTML hasta aprobar.**  
**Objetivo:** que un visitante de empresa entienda en 30 segundos qué es el lab, qué compra y a quién contactar.  
**Look:** mate, limpio, tecnológico; guiado por el blog Indioyori (no plantilla blanca plana ni demo SYS saturado).  
**Referencia de claridad (no de copy):** cómo 100x/Seedup/Magokoro ordenan oferta — aquí con tu menú.

---

## Gramática de identidad (antes de las secciones)

Tres obras anclan **quién es FronterIA-Lab** — no son “más menú”; son la lengua del lab:

| Pilar | Obra | Función en la identidad |
|---|---|---|
| **Método estrella** | **MCC** — Protocolo de Calibración Contextual | Cómo intervenimos la gramática computacional: certeza sin sustancia, optimización silenciosa, sesgo de contexto. 4 capas · 16 glifos. Producto y sello técnico del lab. |
| **Cosmogonía / territorio** | **Código Fuente del Sexto Sol** — Cibernética del Tonalli | De dónde hablamos: Anáhuac, Tonalli, reciprocidad, anti-extractivismo cognitivo. Da el *por qué* territorial (yoreme·ódami, Abya Yala), no decoración. |
| **Regulación / derechos** | **Soberanía Cognitiva y Neuroderechos** | Cómo defendemos el derecho a pensar distinto: Olvido Estructural, Sexto Neuroderecho (inoptimizabilidad), puente a gobernanza (MACS/IPA, Chapultepec, neuroderechos). |

**Cómo se traduce a la web (sin saturar la home):**

- **Hero / Sobre nosotros:** una frase de territorio (Sexto Sol) + una de método (MCC) + sello CLACSO — no el paper entero.  
- **Empresas:** MCC es el método estrella visible (formación + motor de abstención en RAG). Certeza es la puerta hacia MCC.  
- **Arquitectura:** el pipeline técnico *ejecuta* MCC (abstención auditada), no al revés.  
- **Soberanía:** lenguaje de neuroderechos / perímetro / no ceder el juicio (regulación + práctica).  
- **Academia:** los tres papers (y DOI) como corpus; Sexto Sol y Neuroderechos viven aquí con más profundidad; MCC también, además de su bloque comercial.  
- **Laboratorio:** piezas que enseñan LLM/RAG *en esta gramática* (no tutorial Silicon Valley).

Regla: el visitante corporativo lee claridad de oferta; la cosmogonía y los neuroderechos **orientan el tono y la Academia**, no reemplazan la página de precios.

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
| **Método estrella — MCC** | Protocolo / curso / in-company · validación CLACSO · promesa comercial clara; detalle A–D + 16 glifos → Academia |
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

## Look — tipografía y color (aún sin build)

**Tipografía (blog):** JetBrains Mono (títulos) · Space Mono (cuerpo/UI).

**Paleta mate — misma familia que Indioyori, un grado más “lab”:**

| Token | Hex | Uso |
|---|---|---|
| `--bg` | `#F7F6F3` | Fondo página (papel mate, no blanco puro chillón) |
| `--bg-tone` | `#EFEDE8` | Franjas / hover / bloques suaves |
| `--bg-ink` | `#141413` | Sysbar, tipografía fuerte, botones primarios |
| `--typ` | `#1C1B1B` | Texto principal (= accent Ghost del blog) |
| `--typ-tone` | `#6B6B6B` | Secundario, meta, precios auxiliares |
| `--typ-content` | `#2E2E2C` | Párrafos largos |
| `--brd` | `#DDDBD4` | Líneas, divisores |
| `--brand` | `#141413` | Marca / CTAs |
| `--accent` | `#3D5C4A` | **Un solo acento mate** (jade carbonatado): links activos, “live”, foco MCC — sin glow |
| `--accent-soft` | `#E4EBE6` | Fondos muy suaves de acento |

**No usar:** púrpura IA · neón · crema+terracota cliché · negro `#000` puro en todo el canvas · sombras multilayers.

**Atmósfera:** fondo mate + una imagen/textura muy baja opacidad en hero (opcional); el resto tipográfico y limpio.  
**No:** página 100% oscura mineral del demo anterior; **sí:** parentesco claro con Ghost Indioyori.

---

## Decisiones (confirmadas 12 ago 2026)

| # | Decisión | Recomendación | Estado |
|---|---|---|---|
| **D1** | Orden de scroll 0→8 | Hero → Sobre nosotros → **Empresas** → Arquitectura → Soberanía → Academia → Laboratorio → Archivo → Contacto | ✅ confirmado |
| **D2** | Dónde va el detalle MCC (A–D / 16 glifos) | **Academia** (profundidad). En **Empresas**: MCC como método estrella con promesa corta + link “ver protocolo”. | ✅ confirmado |
| **D3** | Cómo vive Laboratorio | Tag/colección **Ghost** (`laboratorio` / lab-notes). Sin WordPress nuevo en cPanel. Home solo destaca + “ver todo”. | ✅ confirmado |
| **D4** | Precios en Empresas | **Sí, precios lista** por servicio (primer nivel). RAG: bandas + “cotización personalizada”. | ✅ confirmado |

### Paquete si dices “ok a todo”

- Nav: `Sobre nosotros` · `Empresas` · `Arquitectura` · `Soberanía` · `Academia` · `Laboratorio` · `Archivo` · `Contacto`
- Identidad: MCC estrella · Sexto Sol (territorio) · Neuroderechos (regulación)
- Look: mate, limpio, tecnológico, guiado por el blog
- Siguiente paso tras confirmar: **copy sección por sección** (aún sin HTML)

Respuesta útil: `ok a todo` **o** `D2=Empresas`, etc.
