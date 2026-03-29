# PROJECT_BRIEF.md — consulta-cata
> Estado actual del proyecto. Actualizar al cierre de cada sesión.

**Última actualización:** 29 marzo 2026 (sesión 1 — cierre)

---

## Cliente

**Catalina Aránguiz Soto** — Psicóloga clínica, atención a pacientes adultos en salud mental.
- Email profesional: `ps.mcaranguiz@gmail.com`
- LinkedIn: https://www.linkedin.com/in/catalina-aranguiz-332661255
- Plataforma de agendamiento: https://encuadrado.com/p/maria-catalina-aranguizv

---

## Stack

| Componente | Tecnología | Estado |
|------------|------------|--------|
| Frontend | HTML/CSS/JS vanilla | Deployado en GitHub Pages |
| Hosting | GitHub Pages (`docs/` branch main) | Activo |
| URL directa | https://ignacio-aranguiz.github.io/consulta-cata/ | Activo |
| Dominio custom | TBD | Pendiente |
| DNS | Cloudflare (Free) | Pendiente |
| Backend formulario | No aplica — usa Encuadrado para agendamiento | — |

---

## URLs y repos clave

- **Repo GitHub:** https://github.com/ignacio-aranguiz/consulta-cata
- **GitHub Pages (URL directa):** https://ignacio-aranguiz.github.io/consulta-cata/
- **Dominio custom:** pendiente

---

## Estado actual (lo que está funcionando HOY)

- [x] Directorio creado: `~/Projects/consulta-cata/`
- [x] Inputs documentados en `inputs/` (docx servicio + CV LinkedIn)
- [x] Landing page v1 completa en `docs/index.html` — 10 secciones
- [x] Repo GitHub creado: `ignacio-aranguiz/consulta-cata`
- [x] GitHub Pages configurado (main / /docs) y activo
- [x] Foto perfil circular en hero (`foto_cata.jpeg`)
- [x] Imagen de fondo hero (`hero-cata.jpeg`) con overlay sage semitransparente
- [ ] Dominio custom comprado
- [ ] DNS configurado (Cloudflare)
- [ ] Valor Fonasa confirmado y actualizado en la web

---

## Contenido del sitio (secciones — estructura consultiva)

1. **Hero** — Propuesta de valor + foto perfil circular + imagen de fondo real
2. **¿Te reconoces?** — Espejo del momento del paciente (antes de hablar de la solución)
3. **Sobre mí** — Credenciales en 4 pilares: formación UC, experiencia clínica, esp. trauma, investigación
4. **Áreas** — 9 áreas de acompañamiento en grid de cards
5. **Cómo trabajo** — 3 pilares metodológicos: integrativo, trauma-informed, mindfulness
6. **El proceso** — 4 pasos del camino terapéutico
7. **Qué puedes esperar** — 5 accordions
8. **Info práctica** — Modalidad, tarifas, lugar (transparente y sin fricción)
9. **FAQ** — 5 preguntas frecuentes en accordion
10. **CTA final** — Llamado empático al primer paso

---

## Diseño

- **Paleta:** verde salvia (`#4A7C5F`) + tierra cálida (`#8A6B52`) + arena (`#F6F1EA`) + blanco
- **Tipografía:** Cormorant Garamond (serif elegante) + Inter (sans limpio)
- **Foto perfil:** `docs/foto_cata.jpeg` — circular en hero
- **Foto de fondo hero:** `docs/hero-cata.jpeg` — con overlay sage semitransparente
- **Agendamiento:** link directo a Encuadrado (no hay formulario propio)

---

## Decisiones tomadas

| Decisión | Razón |
|----------|-------|
| Estructura "McKinsey" (problema antes que solución) | Alta conversión: el paciente se reconoce antes de leer las credenciales |
| Sin formulario propio | Cata ya usa Encuadrado — no duplicar infraestructura |
| Paleta verde salvia (distinta a consuelo-hr) | Identidad propia para salud mental / calma / confianza |
| Accordions para FAQ y "Qué esperar" | Solicitud explícita de Cata en el doc de inputs |
| 4 pilares de credenciales (no solo "titulada UC") | Posiciona la especialización en trauma como diferenciador clave |
| Foto LinkedIn como perfil y hero por ahora | Foto profesional formal pendiente para más adelante |

---

## Pendientes de contenido

- [ ] Confirmar precio Fonasa → actualizar en sección "Info práctica"
- [ ] Decidir dominio (ej. `catalinaaranguiz.cl`, `pscatalina.cl`) → comprar en NIC Chile
- [ ] Foto profesional definitiva (actualmente usa fotos LinkedIn — ok por ahora)

---

## Estructura de archivos

```
consulta-cata/
├── PROJECT_BRIEF.md          ← este archivo
├── docs/
│   ├── index.html            ← landing page (fuente de verdad del frontend)
│   ├── foto_cata.jpeg        ← foto perfil circular (hero)
│   ├── hero-cata.jpeg        ← imagen de fondo hero
│   └── CNAME                 ← (crear cuando se tenga dominio)
└── inputs/
    ├── info_servicio.md      ← contenido extraído del docx de Cata
    └── perfil_catalina.md    ← perfil LinkedIn / CV
```

---

## Workflow de deploy

```bash
cd ~/Projects/consulta-cata
git add docs/index.html
git commit -m "descripción"
git push
# GitHub Pages actualiza en ~30 segundos
```

---

## Próximos 3 pasos

1. **Decidir y comprar dominio** (Ignacio + Cata) → NIC Chile → configurar Cloudflare → agregar CNAME en repo
2. **Confirmar precio Fonasa** (Cata) → actualizar línea correspondiente en `docs/index.html`
3. **Revisar el sitio con Cata** → ajustes de tono, contenido o fotos según su feedback
