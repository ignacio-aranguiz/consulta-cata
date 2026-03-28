# PROJECT_BRIEF.md — consulta-cata
> Estado actual del proyecto. Actualizar al cierre de cada sesión.

**Última actualización:** 28 marzo 2026 (sesión 1)

---

## Cliente

**Catalina Aránguiz Soto** — Psicóloga clínica, atención a pacientes adultos en salud mental.
- Email profesional: `ps.mcaranguiz@gmail.com`
- LinkedIn: https://www.linkedin.com/in/catalina-aranguiz-332661255
- Plataforma de agendamiento: https://encuadrado.com/p/maria-catalina-aranguizv

---

## Stack (objetivo — mismo patrón que consuelo-hr)

| Componente | Tecnología | Estado |
|------------|------------|--------|
| Frontend | HTML/CSS/JS vanilla | Creado, pendiente deploy |
| Hosting | GitHub Pages (`docs/` branch main) | Pendiente |
| Dominio | TBD | Pendiente |
| DNS | Cloudflare (Free) | Pendiente |
| Backend formulario | No aplica — usa Encuadrado para agendamiento | — |

---

## Estado actual

- [x] Directorio creado: `~/Projects/consulta-cata/`
- [x] Inputs documentados en `inputs/`
- [x] Landing page v1 creada en `docs/index.html`
- [ ] Repo GitHub creado
- [ ] GitHub Pages configurado
- [ ] Dominio comprado
- [ ] DNS configurado (Cloudflare)
- [ ] Foto profesional de Cata agregada
- [ ] Valor Fonasa confirmado y actualizado en la web

---

## Contenido del sitio (secciones — estructura consultiva)

1. **Hero** — Propuesta de valor + identidad profesional clara
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
- **Foto:** placeholder circular en hero — pendiente foto real de Catalina
- **Agendamiento:** link directo a Encuadrado (no hay formulario propio)

---

## Decisiones de diseño tomadas

| Decisión | Razón |
|----------|-------|
| Estructura "McKinsey" (problema antes que solución) | Alta conversión: el paciente se reconoce antes de leer las credenciales |
| Sin formulario propio | Cata ya usa Encuadrado — no duplicar infraestructura |
| Paleta verde salvia (distinta a consuelo-hr) | Identidad propia para salud mental / calma / confianza |
| Accordions para FAQ y "Qué esperar" | Solicitud explícita de Cata en el doc de inputs |
| 4 pilares de credenciales (no solo "titulada UC") | Posiciona la especialización en trauma como diferenciador clave |

---

## Pendientes de contenido

- [ ] Foto profesional de Catalina (reemplazar placeholder en hero)
- [ ] Confirmar precio Fonasa
- [ ] Confirmar dominio (¿consulta-cata.cl? ¿catalinaaranguiz.cl? ¿pscatalina.cl?)
- [ ] Verificar email de contacto correcto (ps.mcaranguiz@gmail.com — confirmado en doc inputs)

---

## Estructura de archivos

```
consulta-cata/
├── PROJECT_BRIEF.md          ← este archivo
├── docs/
│   ├── index.html            ← landing page (fuente de verdad del frontend)
│   └── CNAME                 ← (crear cuando se tenga dominio)
└── inputs/
    ├── info_servicio.md      ← contenido extraído del docx de Cata
    └── perfil_catalina.md    ← perfil LinkedIn / CV
```

---

## Workflow de deploy (idéntico a consuelo-hr)

```bash
cd ~/Projects/consulta-cata
git add docs/index.html
git commit -m "descripción"
git push
# GitHub Pages actualiza en ~30 segundos
```

---

## Próximos 3 pasos

1. **Crear repo GitHub** `consulta-cata` y hacer primer push
2. **Conseguir foto profesional** de Catalina para reemplazar el placeholder circular del hero
3. **Decidir dominio** y comprarlo en NIC Chile → configurar Cloudflare → GitHub Pages
