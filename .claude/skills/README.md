# Skills

Colección de skills de Claude Code, migrados desde la instalación local (carpeta `~/.claude/skills`) a este repositorio para poder versionarlos y compartirlos entre máquinas.

Cada subcarpeta es un skill independiente con su propio `SKILL.md`. Claude Code los detecta automáticamente si este repo se abre como proyecto (`.claude/skills/<nombre>/SKILL.md`).

## Origen de cada skill

| Carpeta local original | Skill instalado aquí | Fuente |
|---|---|---|
| VibeSec-Skill | `vibesec-skill` | [BehiSecc/VibeSec-Skill](https://github.com/BehiSecc/VibeSec-Skill) |
| claude-design-auditor-skill-1.2.13 | `claude-design-auditor` | [Ashutos1997/claude-design-auditor-skill](https://github.com/Ashutos1997/claude-design-auditor-skill) |
| prompt-master | `prompt-master` | [nidhinjs/prompt-master](https://github.com/nidhinjs/prompt-master) |
| caveman | `caveman` | [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) |
| caveman-help | `caveman-help` | idem |
| caveman-review | `caveman-review` | idem |
| caveman-commit | `caveman-commit` | idem |
| caveman-compress | `caveman-compress` | idem |
| caveman-stats | `caveman-stats` | idem |
| cavecrew | `cavecrew` | idem |
| absolute-human | `absolute-work` | [AbsolutelySkilled/AbsolutelySkilled](https://github.com/AbsolutelySkilled/AbsolutelySkilled) — el skill se renombró río arriba, `absolute-human` ahora es `absolute-work` |
| absolute-brainstorm | `absolute-spec` | idem — equivalente actual más cercano (spec/diseño antes de construir) |
| clean-code | `clean-code` | [sickn33/antigravity-awesome-skills](https://github.com/sickn33/antigravity-awesome-skills/tree/main/skills/clean-code) |
| codedocs | *(no encontrado)* | No se localizó una fuente pública que coincida con confianza; se omitió |
| find-skills | `find-skills` | [vercel-labs/skills](https://github.com/vercel-labs/skills/tree/main/skills/find-skills) |
| second-brain | `second-brain-*` (6 skills) | [coleam00/second-brain-skills](https://github.com/coleam00/second-brain-skills): brand-voice-generator, mcp-client, pptx-generator, remotion, sop-creator, skill-creator |
| skill-audit | `skill-audit` | [nyosegawa/skills → skill-auditor](https://github.com/nyosegawa/skills/tree/main/skills/skill-auditor) |
| backend-engineering | `backend-*` (12 skills) | [olucasandrade/backend-skills](https://github.com/olucasandrade/backend-skills) — no había un único skill "backend-engineering"; se instaló la suite completa desagregada (security-review, architecture-review, performance-review, api-docs, rfc-review, requirement-gap-analysis, rfc-to-api, rfc-to-schema, er-generator, log-triage, log-triage-interactive, incident-summary) |
| vercel-react-best-practices | `vercel-react-best-practices` | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) |
| web-design-guidelines | `web-design-guidelines` | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) |

## Notas

- **caveman / cavecrew / caveman-*** cambian el estilo de salida de Claude a "modo cavernícola" (respuestas muy comprimidas, en tono tipo "hombre de las cavernas") para ahorrar tokens de salida. Es un cambio de estilo fuerte — actívalo a propósito.
- **codedocs** no se instaló: no encontré una fuente pública inequívoca con ese nombre. Si me puedes pasar el link o el `SKILL.md` original, lo agrego.
- Cada skill conserva su propio `README`/`LICENSE` cuando la fuente lo incluía.

---

## Segunda tanda: creación de contenido/temario + programación

Añadidos a petición explícita para el caso de uso del centro: crear contenido y temarios con Claude Code, más buenas prácticas de programación. Búsqueda abierta, no solo nombres calcados.

### Documentos y contenido de oficina (Anthropic oficial)

Del repo oficial [anthropics/skills](https://github.com/anthropics/skills). La mayoría es Apache 2.0; **docx, pptx, xlsx y pdf son "source-available"** (Anthropic los comparte para referencia, no son open source, pero su uso está explícitamente previsto).

| Skill | Para qué sirve |
|---|---|
| `docx` | Crear/editar documentos Word (temarios, guías, fichas) |
| `pptx` | Crear/editar presentaciones PowerPoint |
| `xlsx` | Hojas de cálculo (notas, seguimiento, planificación) |
| `pdf` | Extraer, combinar, rellenar formularios, OCR de PDFs |
| `doc-coauthoring` | Co-redacción de documentos largos con revisiones |
| `brand-guidelines` | Aplicar una identidad de marca consistente al contenido |
| `theme-factory` | Generar temas visuales/paletas para materiales |
| `canvas-design` | Diseño visual tipo canvas (pósters, infografías) |
| `frontend-design` | Construir interfaces/páginas web con buen criterio de diseño |
| `web-artifacts-builder` | Construir artefactos web interactivos (mini-apps, demos) |

### Creación de temario y contenido pedagógico

De [GarethManning/education-agent-skills](https://github.com/GarethManning/education-agent-skills) (165 skills educativos basados en evidencia científica, licencia CC BY-SA 4.0). Se instaló el subconjunto directamente relevante para diseñar temarios y contenido — el resto de categorías (aprendizaje socioemocional, alfabetización, etc.) no se instalaron pero están disponibles en el repo original si las quieres luego.

- **Diseño curricular** (`edu-scope-and-sequence-designer`, `edu-backwards-design-unit-planner`, `edu-curriculum-knowledge-architecture-designer`, `edu-learning-progression-builder`, `edu-competency-unpacker`, `edu-kud-knowledge-type-mapper`, `edu-project-brief-designer`, `edu-discipline-specific-critical-thinking-task-designer`, `edu-differentiation-adapter`)
- **Evaluación** (`edu-criterion-referenced-rubric-generator`, `edu-formative-assessment-technique-selector`, `edu-assessment-validity-checker`, `edu-gap-analysis-from-student-work`)
- **Alineación curricular** (`edu-coverage-audit`, `edu-curriculum-crosswalk`, `edu-developmental-band-translator`, `edu-kud-chart-author`)
- **Diseño de instrucción explícita** (`edu-explicit-instruction-sequence-builder`, `edu-lesson-opening-designer`, `edu-practice-problem-sequence-designer`, `edu-think-aloud-script-generator`, `edu-checking-for-understanding-protocol-designer`)
- **Preguntas y discusión en clase** (`edu-socratic-questioning-sequence-generator`, `edu-hinge-question-designer`, `edu-dialogic-teaching-move-generator`, `edu-discussion-protocol-selector`, `edu-perspective-taking-designer`)

### Flujo de trabajo de programación

De [obra/superpowers](https://github.com/obra/superpowers) (MIT, ~41k estrellas — la colección de skills de programación más usada de la comunidad). Prefijo `superpowers-` para no chocar con nombres genéricos:

`superpowers-brainstorming`, `superpowers-writing-plans`, `superpowers-executing-plans`, `superpowers-test-driven-development`, `superpowers-systematic-debugging`, `superpowers-using-git-worktrees`, `superpowers-finishing-a-development-branch`, `superpowers-requesting-code-review`, `superpowers-receiving-code-review`, `superpowers-subagent-driven-development`, `superpowers-dispatching-parallel-agents`, `superpowers-verification-before-completion`, `superpowers-writing-skills`, `superpowers-using-superpowers`

Más de Anthropic oficial: `webapp-testing` (probar apps web end-to-end), `mcp-builder` (crear servidores MCP propios), `claude-api` (referencia de la API de Claude/Anthropic).

### Moodle (desarrollo)

De [SaadRahman01/claude-moodle-dev](https://github.com/SaadRahman01/claude-moodle-dev) (MIT). Instalado por completo porque esta sesión ya tiene conectado un MCP de Moodle — útil si el centro desarrolla plugins, temas o integraciones sobre su propio Moodle:

`moodle-plugin-development`, `moodle-theme-development`, `moodle-hooks-api`, `moodle-web-services`, `moodle-amd-javascript`, `moodle-mobile-app`, `moodle-upgrade-migration`, `moodle-phpunit-testing`, `moodle-behat-testing`, `moodle-security-audit`, `moodle-privacy-gdpr`, `moodle-accessibility`, `moodle-performance`

### Recomendado pero no instalado

- **[zarazhangrui/codebase-to-course](https://github.com/zarazhangrui/codebase-to-course)** — convierte un repo de código en un curso interactivo HTML de una sola página (ideal si enseñáis programación a partir de proyectos reales). No lo copié al repo porque no tiene licencia declarada; si os interesa, puedo instalarlo igualmente o simplemente clonarlo aparte.
