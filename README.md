# Descriprion
PoC use antigravity agent to create presentations using OpenSpec

## STEPS

- **STEP01**
Create your default working folder
```bash
mkdir my-presentation
cd my-presentation
```

- **STEP02**
Initialize OpenSpec in your working folder. After this you will have your `.agent` folder with all openspec skills and the `openspec` folder used by OpenSpec to implement SDD

```bash
openspec init
```

- **STEP03**
Install the pptx skill from Anthropic to create any type of presentations. We will use the tool called `openskills` with the argument universal because our agent is not the default agent used by this Anthropic tool. With this argument the skill will installed inside `.agent` folder and not `.claude`. The inside we can select the skill `pptx` to be installed.

```bash
npx openskills install anthropics/skills --universal
Need to install the following packages:
openskills@1.5.0
Ok to proceed? (y) y

Installing from: anthropics/skills
Location: project (.agent/skills)
Default install is project-local (./.agent/skills). Use --global for ~/.agent/skills.

✔ Repository cloned
Found 20 skill(s)

? Select skills to install
 ◉ discernment-nudge         21.4KB
 ◉ doc-coauthoring           15.4KB
 ◉ docx                      1.1MB
 ◉ frontend-design           19.1KB
 ◉ internal-comms            21.9KB
 ◉ mcp-builder               118.9KB
 ◉ pdf                       57.3KB
❯◉ pptx                      1.1MB
 ◉ skill-creator             219.7KB
 ◉ slack-gif-creator         42.7KB
 ◉ theme-factory             140.7KB
 ◉ web-artifacts-builder     44.8KB
 ◉ webapp-testing            21.9KB
 ◉ xlsx                      1.1MB
 ◉ template                  140B

"Use this skill any time a .pptx or .potx file is involved in any way — as input
↑↓ navigate • space select • a all • i invert • ⏎ submit
```

- **STEP04**
Start your agent inside your working folder, in our case antigravity:

```bash
agy

                  Antigravity CLI 1.2.16
                  masalinas.gancedo@gmail.com (Google AI Pro)
                  Gemini 3.8 Flash (High)
                  ~/git/sqlserver-training
              

> /skills
  ⎿  Exited /skills command

────────────────────────────────────────────────────────────
────────────────────────────────────────────────────────────
```

- **STEP05**
Now you can start to implement your presentation. This is a sample not using open

```bash
────────────────────────────────────────────────────────────
> /openspec-explore\
Usa la skill pptx para crear una presentación de 3 slides sobre la arquitectura básica de SQL Server en presentaciones/prueba/. Cuando termines, renderízala a imágenes y revisa que no haya texto desbordado ni solapamientos.
────────────────────────────────────────────────────────────
```
