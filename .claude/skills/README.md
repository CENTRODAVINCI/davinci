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
