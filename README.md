<h1 align="center">Mateus Vidal</h1>

<p align="center">
  Front-end developer. Design systems, TypeScript, React.
</p>

<p align="center">
  <sub>I build the layer between what a design promises and what the browser actually ships.</sub>
</p>

---

Design was my way into engineering. That still shows up in how I work: I notice the
4px problem, and I also know what it costs to fix it properly instead of nudging a
margin. But the code is the job now. I write production TypeScript, own front-end
architecture, and spend most of my thinking on the system rather than the screen.

If I have one habit worth hiring, it's this: when something breaks twice the same way,
I stop patching instances and go fix the cause. Usually that means the system was
missing a piece.

I'm in the middle of a deliberate shift right now, from building interfaces to
engineering them. Past the stage where tools do my thinking. Still filling in
fundamentals, on purpose.

## How I work

Design systems are code to me, not a Figma page. I build tokens in two tiers so call
sites reference intent rather than a hex value, and I put new patterns into the shared
layer before any screen uses them. It's slower for the first two screens and much
faster for the next twenty.

Abstraction has to earn itself. Two hardcoded values in two files means a token is
missing. One value doesn't mean anything yet.

Accessibility I treat as a build-time constraint. Contrast, visible focus, reduced
motion. It's cheap as a requirement and expensive as a retrofit, and I don't ship past it.

I work from numbers, not screenshots. Exact values from the source, not a rendered PNG
and a guess. This removes a whole category of arguing with designers about whether
something is "close enough."

Where a design and an established system disagree, the system wins and the design
adapts. That's what keeps twenty pages looking like one product.

And I write things down as I go — architecture notes, conventions, the reasoning behind
anything non-obvious. Partly for whoever comes next. Mostly for me in six months.

```mermaid
flowchart LR
    A[Design intent] --> B[Tokens]
    B --> C[Shared components]
    C --> D[Screens]
    D --> E[Validation]
    E -->|fix the cause| B
```

## The stack

<table>
<tr>
<td valign="top" width="180">
<strong>Daily</strong><br>
<sub>I reach for these<br>without thinking</sub>
</td>
<td valign="top">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
<img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React">
<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5">
<img src="https://img.shields.io/badge/CSS-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS">
<img src="https://img.shields.io/badge/Design%20Tokens-4C4C4C?style=flat-square" alt="Design Tokens">
<img src="https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white" alt="Astro">
<img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite">
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">
<img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub">
<img src="https://img.shields.io/badge/Figma-F24E1E?style=flat-square&logo=figma&logoColor=white" alt="Figma">
<img src="https://img.shields.io/badge/Webflow-146EF5?style=flat-square&logo=webflow&logoColor=white" alt="Webflow">
<img src="https://img.shields.io/badge/VS%20Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white" alt="VS Code">
</td>
</tr>
<tr>
<td valign="top">
<strong>Comfortable</strong><br>
<sub>solid working knowledge,<br>used when the job needs it</sub>
</td>
<td valign="top">
<img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js">
<img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white" alt="Express">
<img src="https://img.shields.io/badge/REST%20APIs-6B7280?style=flat-square" alt="REST APIs">
<img src="https://img.shields.io/badge/OAuth2%20%2F%20PKCE-6B7280?style=flat-square" alt="OAuth2 / PKCE">
<img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase">
<img src="https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white" alt="Google Cloud">
<img src="https://img.shields.io/badge/GSAP-0AE448?style=flat-square&logo=greensock&logoColor=black" alt="GSAP">
<img src="https://img.shields.io/badge/Radix%20UI-161618?style=flat-square&logo=radixui&logoColor=white" alt="Radix UI">
<img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" alt="Playwright">
<img src="https://img.shields.io/badge/WCAG%20AA-6B7280?style=flat-square" alt="WCAG AA">
</td>
</tr>
<tr>
<td valign="top">
<strong>Learning now</strong><br>
<sub>actively in progress,<br>not claiming these yet</sub>
</td>
<td valign="top">
<img src="https://img.shields.io/badge/GitHub%20Actions%20%26%20CI%2FCD-D9A227?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions and CI/CD">
<img src="https://img.shields.io/badge/Automated%20testing-D9A227?style=flat-square&logo=vitest&logoColor=white" alt="Automated testing">
<img src="https://img.shields.io/badge/Algorithms%20%26%20data%20structures-D9A227?style=flat-square" alt="Algorithms and data structures">
</td>
</tr>
</table>

The third row is the honest one. I could pad the top row with everything I've touched
once, but a lead who hires on that list finds out in week two.

## What I'm fixing in myself

The JavaScript pass I'm doing now is the deep one, not the tutorial one. Event loop,
closures, prototypes, why React behaves the way it does under the hood.

Testing is where I'm thinnest. I've historically validated visually and by hand, which
works right up until it doesn't. Building real testing discipline is my current project,
and I'd rather tell you than have you find it in a code review.

I'm also learning to treat the pipeline as part of the product. Automated checks,
reproducible builds, deploys that aren't a manual ritual.

Last one: I'm reading more code than I write. Nothing has improved my engineering faster
than studying a well-architected codebase instead of only producing my own.

## On AI tools

I use them heavily and I think the how matters more than the whether.

I build tooling rather than paste output — reusable workflows and documented project
context, so what comes back is grounded in the actual codebase. Anything automated
proposes; nothing writes to source unsupervised. And I own every line that ships. If I
can't explain it, it doesn't go in. Speed bought against understanding isn't speed.

## Fit

I do my best work where design precision and front-end architecture overlap. Design
systems, component architecture, motion, accessibility, interfaces that have to survive
real product complexity. I want a team that writes things down and gives blunt feedback.

If you're a lead sizing me up: I'm strong on design-to-code quality and system thinking,
I'm honest about the depth I'm still building, and I take "the standard is higher than
that" well.

---

<p align="center">
  <a href="https://mattvidal.works/"><img src="https://img.shields.io/badge/Portfolio-mattvidal.works-111111?style=flat-square" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/mateusvidal/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
</p>

<p align="center">
  <sub>Open to conversations about front-end and design-systems work.</sub>
</p>
