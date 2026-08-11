# Sitios web — diagnóstico y unificación

**Corte:** 11 agosto 2026  
**URLs:** `fronteria-lab.com` · `indioyori.fronteria-lab.com` · (tercer canal) `demvk.substack.com`

---

## 1. Estado actual (hechos)

| Sitio | Plataforma | Estado | Rol hoy |
|---|---|---|---|
| **fronteria-lab.com** | Namecheap cPanel · HTML estático (`public_html/index.html`) | **CAÍDO** — sin registro A; DNS en `registrar-servers.com` | Debía ser landing del lab |
| **indioyori.fronteria-lab.com** | **Ghost** (`indioyori.ghost.io` + Fastly) | **Vivo** | Voz + blog + talleres + membresía $350 MXN |
| **demvk.substack.com** | Substack | Vivo | Blog paralelo (tercer canal) |

### DNS / correo (problema crítico)

| Registro | Valor actual | Problema |
|---|---|---|
| NS `fronteria-lab.com` | `dns1/dns2.registrar-servers.com` | No es Web Hosting DNS (`namecheaphosting.com`) que pedía el setup TEKTRON |
| A `fronteria-lab.com` | **no existe** | Por eso “Could not resolve host” |
| `indioyori` | CNAME → `indioyori.ghost.io` | OK (Ghost Pro) |
| MX | `mx1/mx2.privateemail.com` | Sigue Private Email; el LEEME pedía cancelar OX y usar correo cPanel Local |

**Sin arreglar DNS del apex, no hay unificación posible.** El blog Ghost puede seguir, pero el lab “oficial” está invisible.

### Ghost (indioyori) — inventario

**Páginas:** Manifiesto · Talleres · Archivo · Comunidad · Contacto (contacto casi vacío en API).  
**Oferta en /talleres:** membresía $350 MXN/mes · Taller MCC · Formación RAG de Borde ~16 h · cotización a la medida.  
**Blog:** mezcla análisis geopolítico (Ormuz, Argentina, China…) + piezas de formación/MCC.  
**Extras:** RSS, llms.txt, Chat Matrix, Suscribirse.

### Desalineación con la estrategia soberanía (07)

| Estrategia acordada | Sitio hoy |
|---|---|
| Capa común gratis (guía, papers) | No hay CTA claro a la guía *IA, Poder y Autonomía* |
| Taller **Certeza** como ancla de entrada | No aparece; sí MCC y RAG (más arriba en la escalera) |
| FronterIA-Lab = MACS / IPA / TEKTRON | Apex caído; no hay SKUs lab |
| Indioyori = voz / commons | Ghost sí, pero vende también formación (OK) y se mezcla con geopolítica sin secciones |
| Un solo blog | Ghost + Substack = doble trabajo |

---

## 2. Arquitectura unificada (recomendación)

Alineada a marca dual ya decidida:

```
fronteria-lab.com              →  LAB (comercial + ecosistema)
  /                            →  Home 3 capas (común / guiada / intervención)
  /ofertas                     →  Certeza · MCC · MACS · TEKTRON (precios)
  /contacto                    →  Cal.com / form → indioyori@ / ragflow@
  /blog  ──redirect──►         indioyori.fronteria-lab.com

indioyori.fronteria-lab.com    →  VOZ + COMÚN (Ghost)
  /                            →  Blog + manifiesto
  /manifiesto                  →  Ya existe
  /guia                        →  Guía gratuita (PDF) — capa común
  /talleres                    →  Solo ofertas de formación (Certeza, MCC…)
  /archivo                     →  Papers / descarga libre
  Tags: formacion | analisis | soberania
```

**Substack:** redirigir lectores a Ghost; no publicar en dos lados. RSS de Ghost = fuente única.

---

## 3. Qué va en cada casa (para no mezclar)

| Contenido | Dónde |
|---|---|
| Manifiesto, análisis, Lives, guía gratis, papers | **Ghost (Indioyori)** |
| One-pagers, precios, SOW, CTA “contratar taller/MACS/TEKTRON” | **Apex FronterIA-Lab** |
| Membresía $350 / comunidad Matrix | Ghost (ya está) — o mover luego |
| Keynote / voz personal | Indioyori |
| Factura lab / B2B | FronterIA-Lab |

---

## 4. Automatización (realista, poca pieza)

| Flujo | Cómo |
|---|---|
| **Un solo blog** | Publicar solo en Ghost · Substack en pausa o import + redirect |
| **Newsletter** | Ghost Members (ya tiene Suscribirse) — un listado |
| **Nuevo post → redes** | Zapier/Make: Ghost webhook → buffer/draft (opcional) |
| **Lead guía gratis** | Página `/guia` + botón PDF · opcional email gate Ghost |
| **Contratar taller** | CTA → Cal.com o form → correo · SOW en PDF |
| **Pago** | Stripe/Mercado Pago links en /talleres y apex /ofertas |
| **Repo → web** | Papers/guía en GitHub Releases o Google Drive link estable en /archivo — no subir ZIP a mano cada vez |
| **Monitoreo** | UptimeRobot gratis en `fronteria-lab.com` + Ghost |

No hace falta un CMS nuevo. **Ghost ya es el cerebro editorial.** El apex es landing comercial (HTML o una página Ghost custom domain si más adelante unifican hosting).

---

## 5. Plan de arreglo (orden estricto)

### Paso 0 — Urgente (DNS / correo) — tú en Namecheap
1. Entrar a Namecheap → Domain List → `fronteria-lab.com`.  
2. Decidir correo **antes** de tocar NS:
   - Si sigues con **Private Email**: deja MX Private Email y pon solo registros A/CNAME web.  
   - Si vuelves a **cPanel mail** (como LEEME): NS → Web Hosting DNS + Email Routing Local + cancelar OX.  
3. Restaurar web apex:
   - Opción rápida: A record → `66.29.132.93` (si el hosting Stellar sigue activo) **o** NS a `dns1/dns2.namecheaphosting.com`.  
4. Verificar: `dig fronteria-lab.com A` + abrir https://fronteria-lab.com.  
5. Confirmar que `indioyori` CNAME a `indioyori.ghost.io` **no se rompe**.

### Paso 1 — Home Lab (apex)
Página mínima con el ecosistema de 3 capas + 4 CTAs:
- Descargar guía (común)
- Taller Certeza / Keynote
- MACS
- TEKTRON / RAG  
Link fijo: “Archivo y blog → indioyori.fronteria-lab.com”

### Paso 2 — Ghost alineado
1. Crear/rellenar **Contacto**.  
2. Añadir página **Guía gratuita** (PDF).  
3. En /talleres: poner **Certeza** arriba; MCC y RAG como siguientes.  
4. Tags: `formacion` vs `analisis` (geopolítica no compite en el menú de venta).  
5. Nav: Inicio · Manifiesto · Guía · Talleres · Archivo · Blog · Contacto.

### Paso 3 — Apagar duplicados
1. No más posts nuevos en Substack.  
2. Pin en Substack: “Nos mudamos a indioyori.fronteria-lab.com”.  
3. Un solo correo público de voz: `indioyori@fronteria-lab.com`.

### Paso 4 — Automatizar
1. Ghost Members = lista.  
2. Links de pago en talleres.  
3. Cal.com “15 min / cotización”.  
4. Uptime en apex.

---

## 6. Criterio de “unificado y automatizado” (hecho)

- [ ] `fronteria-lab.com` resuelve y muestra home lab  
- [ ] `indioyori.` sigue en Ghost sin error  
- [ ] Un solo blog activo  
- [ ] Guía gratis enlazada desde ambos  
- [ ] /talleres muestra Certeza → MCC → RAG  
- [ ] Contacto con form o Cal.com que llega a tu correo  
- [ ] Correo (Private Email **o** cPanel) estable y documentado  
- [ ] No hay tercer sitio pidiendo mantenimiento semanal  

---

## 7. Lo que no puedo hacer yo sin tu acceso

- Entrar a Namecheap / cPanel / Ghost Admin / Private Email.  
- Subir el `index.html` al `public_html`.  
- Cambiar DNS.

Si me das acceso (o haces el Paso 0), el siguiente entregable es el **HTML de la home lab** + copy listo para pegar en Ghost (Guía, Contacto, orden de Talleres).
