<!-- Repo name must match your username exactly: nbucci4325/nbucci4325 -->

<div align="center">

<img src="assets/hero.svg" alt="Nico, Game Programmer" width="100%" />

<a href="https://github.com/nbucci4325">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3200&pause=1000&color=00F0FF&center=true&vCenter=true&width=700&height=40&lines=Building+gameplay+systems+in+Unity+%26+C%23;Evolving+AI+with+genetic+algorithms;Shipping+tools+other+devs+actually+use;Looking+for+my+next+co-op" alt="Typing tagline" />
</a>

<a href="https://www.linkedin.com/in/YOUR-LINKEDIN"><img src="https://img.shields.io/badge/LinkedIn-0d1117?style=for-the-badge&logo=linkedin&logoColor=00F0FF" alt="LinkedIn" /></a>
<a href="mailto:YOUR@EMAIL.COM"><img src="https://img.shields.io/badge/Email-0d1117?style=for-the-badge&logo=gmail&logoColor=FF2E97" alt="Email" /></a>
<img src="https://img.shields.io/badge/CO--OP-OPEN-0d1117?style=for-the-badge&labelColor=0d1117&color=39ff88" alt="Open to co-op" />

<br /><br />

<img src="assets/terminal.svg" alt="Terminal: whoami" width="90%" />

</div>

<img src="assets/divider.svg" width="100%" alt="" />

## ⚡ About

I build gameplay systems and AI behavior, mostly in **C# and Unity**. I like tools that make other developers faster, and I enjoy applying algorithms, especially **genetic algorithms**, to real problems.

<details>
<summary><b>🎮 Press START: character sheet</b></summary>

<br />

```text
┌──────────────────────────────────────────┐
│  PLAYER      Nico                        │
│  CLASS       Game Programmer             │
│  GUILD       Brock / Niagara College     │
│  MAIN HAND   C# / Unity                  │
│  OFF HAND    Python                      │
│  SPELLBOOK   Genetic Algorithms, FSMs    │
│  QUEST       Land a co-op                │
│  STATUS      ● Open to party invites     │
└──────────────────────────────────────────┘
```

</details>

<img src="assets/divider.svg" width="100%" alt="" />

## 🧰 Tech

<div align="center">
  <img src="https://skillicons.dev/icons?i=cs,dotnet,unity,python,java,mysql&theme=dark" alt="Languages and engines" />
  <br />
  <img src="https://skillicons.dev/icons?i=git,github,githubactions,vscode,visualstudio,discord&theme=dark" alt="Tools" />
</div>

<img src="assets/divider.svg" width="100%" alt="" />

## 🧠 Game AI, in one diagram

```mermaid
%%{init: {'theme':'base','themeVariables':{'background':'#0d1117','primaryColor':'#140a3a','primaryTextColor':'#e6faff','primaryBorderColor':'#00f0ff','lineColor':'#ff2e97','secondaryColor':'#1b1b3a','tertiaryColor':'#0d1117','edgeLabelBackground':'#0d1117','textColor':'#c9d1d9','fontFamily':'monospace'}}}%%
stateDiagram-v2
    direction LR
    [*] --> Patrol
    Patrol --> Chase: player spotted
    Chase --> Attack: in range
    Attack --> Chase: out of range
    Chase --> Search: lost sight
    Search --> Patrol: timeout
    Search --> Chase: player spotted
    Attack --> Flee: low health
    Flee --> Patrol: safe
```

<img src="assets/divider.svg" width="100%" alt="" />

## 🚀 Projects

<table>
  <tr>
    <td width="50%">
      <a href="https://github.com/nbucci4325/StockGA">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=nbucci4325&repo=StockGA&bg_color=0d1117&title_color=00F0FF&text_color=c9d1d9&icon_color=FF2E97&border_color=30363d" alt="StockGA" />
      </a>
    </td>
    <td width="50%">
      <a href="https://github.com/nbucci4325/UNITY-UTILITIES-REPO">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=nbucci4325&repo=UNITY-UTILITIES-REPO&bg_color=0d1117&title_color=00F0FF&text_color=c9d1d9&icon_color=FF2E97&border_color=30363d" alt="Unity Utilities" />
      </a>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <a href="https://github.com/nbucci4325/UML-DESIGNER-REPO">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=nbucci4325&repo=UML-DESIGNER-REPO&bg_color=0d1117&title_color=00F0FF&text_color=c9d1d9&icon_color=FF2E97&border_color=30363d" alt="UML Designer" />
      </a>
    </td>
    <td width="50%">
      <a href="https://github.com/nbucci4325/SHOWTIME-BOT-REPO">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=nbucci4325&repo=SHOWTIME-BOT-REPO&bg_color=0d1117&title_color=00F0FF&text_color=c9d1d9&icon_color=FF2E97&border_color=30363d" alt="Showtime Bot" />
      </a>
    </td>
  </tr>
</table>

<details>
<summary><b>🧬 StockGA: how the evolution loop works</b></summary>

<br />

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#140a3a','primaryTextColor':'#e6faff','primaryBorderColor':'#00f0ff','lineColor':'#ff2e97','edgeLabelBackground':'#0d1117','textColor':'#c9d1d9','fontFamily':'monospace'}}}%%
flowchart LR
    A([Random population of signal parameters]) --> B[Evaluate fitness: cumulative return]
    B --> C[Select parents]
    C --> D[Uniform crossover]
    D --> E[Mutate]
    E --> B
    B -. best individual .-> F([Trading signal])
```

</details>

<details>
<summary><b>♻️ Unity Utilities: object pool lifecycle</b></summary>

<br />

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#140a3a','primaryTextColor':'#e6faff','primaryBorderColor':'#00f0ff','lineColor':'#ff2e97','edgeLabelBackground':'#0d1117','textColor':'#c9d1d9','fontFamily':'monospace'}}}%%
stateDiagram-v2
    direction LR
    [*] --> Inactive: Pool created
    Inactive --> Active: Get(position, rotation)
    Active --> Inactive: Release()
```

</details>

<details>
<summary><b>📦 Everything else I've built</b></summary>

<br />

- **StockGA:** genetic algorithm in Python evolving trading signal parameters, integrated with a neural network pipeline.
- **Unity Utilities:** generic `Singleton<T>`, typed object pools and a min/max slider Inspector drawer.
- **UML Designer:** PySide6 desktop app with undo/redo and automated PyInstaller releases.
- **Showtime Bot:** Discord bot with alerts, deployed with GitHub Actions.

</details>

<img src="assets/divider.svg" width="100%" alt="" />

## 📈 Stats

<table>
  <tr>
    <td width="50%" align="center">
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=nbucci4325&layout=compact&hide_border=true&bg_color=0d1117&title_color=00F0FF&text_color=c9d1d9" alt="Top languages" />
    </td>
    <td width="50%" align="center">
      <img src="https://streak-stats.demolab.com?user=nbucci4325&background=0D1117&ring=FF2E97&fire=FF2E97&currStreakLabel=00F0FF&currStreakNum=FFFFFF&sideNums=FFFFFF&sideLabels=00F0FF&dates=7D8AA8&stroke=30363D&border=00000000" alt="Streak" />
    </td>
  </tr>
</table>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=nbucci4325&bg_color=0d1117&color=00f0ff&line=ff2e97&point=ffffff&area=true&area_color=3a0ca3&hide_border=true&custom_title=Contribution%20Activity" alt="Activity graph" width="100%" />
  <br />
  <img src="https://raw.githubusercontent.com/nbucci4325/nbucci4325/output/snake-neon.svg" alt="Contribution snake" width="100%" />
</div>

<details>
<summary><b>🛠️ Currently working on</b></summary>

<br />

- Replace this with 2–3 short bullets.

</details>

<div align="center">
<br />
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=14&duration=4000&pause=1500&color=7D8AA8&center=true&vCenter=true&width=500&height=30&lines=Thanks+for+stopping+by.;Let's+build+something+fun." alt="Sign-off" />
<br />
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00f0ff,50:3a0ca3,100:0d1117&height=110&section=footer" alt="Footer" width="100%" />
</div>
