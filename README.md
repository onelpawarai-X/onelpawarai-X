import pypandoc

readme = r'''<div align="center">

<a href="https://github.com/onelpawarai-X/ZYRAXON-AI">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=250&section=header&text=ZYRAXON%20AI&fontSize=68&fontColor=FFFFFF&fontAlignY=38&animation=twinkling&color=0:030712,35:071B3A,70:312E81,100:0891B2" width="100%" alt="ZYRAXON AI animated banner"/>
</a>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=19&duration=2600&pause=800&color=38BDF8&center=true&vCenter=true&width=850&lines=AUTONOMOUS+AI+AGENT+ENGINEERING;10+BRANDED+MODELS.+ONE+PROVIDER.;REASON+%E2%80%A2+EXECUTE+%E2%80%A2+OBSERVE+%E2%80%A2+VERIFY;OPEN+SOURCE+%C2%B7+MULTIMODAL+%C2%B7+DEVELOPER+FIRST" alt="Animated ZYRAXON AI tagline"/>

<br/>

<a href="https://zyraxonai.lovable.app/"><img src="https://img.shields.io/badge/EXPLORE-ZYRAXON%20AI-071B3A?style=for-the-badge&logo=openai&logoColor=38BDF8" alt="Explore ZYRAXON AI"/></a>
<a href="https://zyraxonai.lovable.app/providers"><img src="https://img.shields.io/badge/MODEL%20PROVIDER-10%20BRANDED%20MODELS-312E81?style=for-the-badge&logo=googlecloud&logoColor=FFFFFF" alt="Model Provider"/></a>
<a href="https://zyraxonai.lovable.app/docs/provider-overview"><img src="https://img.shields.io/badge/DEVELOPER-DOCUMENTATION-164E63?style=for-the-badge&logo=readthedocs&logoColor=FFFFFF" alt="Documentation"/></a>
<a href="https://github.com/onelpawarai-X/ZYRAXON-AI"><img src="https://img.shields.io/badge/OPEN%20SOURCE-VIEW%20THE%20CODE-0B1220?style=for-the-badge&logo=github&logoColor=FFFFFF" alt="Source code"/></a>

<br/><br/>

<a href="https://github.com/onelpawarai-X/ZYRAXON-AI"><img src="https://img.shields.io/github/stars/onelpawarai-X/ZYRAXON-AI?style=flat-square&color=38BDF8&label=STARS" alt="GitHub stars"/></a>
<a href="https://github.com/onelpawarai-X/ZYRAXON-AI"><img src="https://img.shields.io/github/forks/onelpawarai-X/ZYRAXON-AI?style=flat-square&color=8B5CF6&label=FORKS" alt="GitHub forks"/></a>
<a href="https://github.com/onelpawarai-X/ZYRAXON-AI"><img src="https://img.shields.io/github/license/onelpawarai-X/ZYRAXON-AI?style=flat-square&color=A78BFA" alt="License"/></a>
<a href="https://komarev.com/ghpvc/?username=onelpawarai-X"><img src="https://komarev.com/ghpvc/?username=onelpawarai-X&style=flat-square&color=0891B2&label=PROFILE+VIEWS" alt="Profile views"/></a>

### INTELLIGENCE IS MORE THAN AN ANSWER.

**Building AI systems that can reason, use tools, execute workflows, and verify outcomes.**

*An open-source AI engineering project exploring autonomous agents, model orchestration, and developer-focused AI infrastructure.*

[Explore the Platform](https://zyraxonai.lovable.app/) · [Explore the Repository](https://github.com/onelpawarai-X/ZYRAXON-AI) · [Explore the Model Provider](https://zyraxonai.lovable.app/providers)

</div>

---

## ◈ THE VISION

AI should do more than generate text. A useful AI system should be able to understand a goal, plan the steps, select suitable tools, act on results, recover from errors, and verify whether the task was completed.

**ZYRAXON AI is built around that engineering philosophy.**

The project brings together autonomous-agent workflows, tool integrations, model orchestration, multimodal interactions, and developer-oriented infrastructure in an evolving ecosystem.

## ◈ ZYRAXON MODEL PROVIDER

<div align="center">

### TEN BRANDED MODELS. ONE UNIFIED API.

**A familiar OpenAI-compatible interface for the ZYRAXON model family.**

<a href="https://zyraxonai.lovable.app/providers"><img src="https://img.shields.io/badge/EXPLORE-MODEL%20CATALOGUE-312E81?style=for-the-badge" alt="Explore model catalogue"/></a>
<a href="https://zyraxonai.lovable.app/docs/provider-overview"><img src="https://img.shields.io/badge/READ-PROVIDER%20DOCS-0891B2?style=for-the-badge" alt="Provider documentation"/></a>

</div>

The ZYRAXON Model Provider presents ten branded model identities through a unified API interface. Developers can use familiar chat-completion patterns and consult the live provider catalogue for current model availability and supported capabilities.

**Provider highlights**
- **Unified API interface** for model discovery and chat completions.
- **Ten branded model identities** for different intended workloads.
- **Streaming-oriented workflows** where supported by the endpoint.
- **Multimodal request formats** for supported media and model combinations.
- **Capability-aware routing and fallback behavior**, as described by the provider documentation.

### API endpoints

| Operation | Endpoint |
|---|---|
| API base URL | `https://zyraxonai.lovable.app/api/public/zyraxon/v1` |
| List models | `GET /models` |
| Chat completions | `POST /chat/completions` |

**List available models**
```http
GET https://zyraxonai.lovable.app/api/public/zyraxon/v1/models
```

**Create a chat completion**
```http
POST https://zyraxonai.lovable.app/api/public/zyraxon/v1/chat/completions
```

### The ten-model lineup

| Model | Intended focus | Advertised context |
|---|---|---:|
| **ZYRAXON Apex** | Flagship reasoning | 1M tokens |
| **ZYRAXON Matrix** | Vision and reasoning | 1M tokens |
| **ZYRAXON Pulse** | Low-latency, long-input tasks | 262K tokens |
| **ZYRAXON Titan** | Long outputs and multimodal workloads | 1M tokens |
| **ZYRAXON Neural** | General-purpose reasoning | 200K tokens |
| **ZYRAXON Codex** | Code generation and repair | 200K tokens |
| **ZYRAXON Visionary** | Image, video, and PDF workflows | 200K tokens |
| **ZYRAXON Cyber** | Text and supported media workflows | 200K tokens |
| **ZYRAXON Quantum** | Long-document reasoning | 1M tokens |
| **ZYRAXON Genesis** | Experimental capabilities | 200K tokens |

*Context sizes and modality labels reflect the supplied provider specifications. Check the live catalogue for current availability, limits, and supported features.*

### Quickstart — JavaScript

Install the OpenAI JavaScript SDK:

```bash
npm install openai
```

Example client setup:

```javascript
import OpenAI from "openai";

const client = new OpenAI({
  baseURL: "https://zyraxonai.lovable.app/api/public/zyraxon/v1",
  apiKey: process.env.ZYRAXON_API_KEY || "not-needed",
});

const response = await client.chat.completions.create({
  model: "zyraxon-apex",
  messages: [
    {
      role: "user",
      content: "Explain how an autonomous AI agent works.",
    },
  ],
});

console.log(response.choices[0].message.content);
```

> **Authentication:** This example follows the supplied public quickstart pattern. Verify the endpoint's current authentication requirements, rate limits, and access policy in the official documentation before using it in production. Never expose a private API key in client-side code.

**Provider links:** [Model Dashboard](https://zyraxonai.lovable.app/providers) · [Quickstart](https://zyraxonai.lovable.app/providers#quickstart) · [Provider Documentation](https://zyraxonai.lovable.app/docs/provider-overview)

---

## ◈ MULTIMODAL AI

### Text and supported media, depending on the selected model

| Modality | Example workflows |
|---|---|
| **Text** | Questions, explanations, and structured responses |
| **Images** | Visual interpretation and chart analysis |
| **Audio** | Supported audio-input workflows |
| **Video** | Video understanding with supported processing |
| **Documents** | PDF and document analysis where supported |

### Example — vision request

```javascript
const response = await client.chat.completions.create({
  model: "zyraxon-matrix",
  messages: [
    {
      role: "user",
      content: [
        { type: "text", text: "Describe the chart and its main trend." },
        {
          type: "image_url",
          image_url: {
            url: "data:image/png;base64,YOUR_IMAGE_BASE64",
          },
        },
      ],
    },
  ],
});

console.log(response.choices[0].message.content);
```

Replace `YOUR_IMAGE_BASE64` with a valid image payload. Confirm supported formats, payload limits, and model compatibility in the provider documentation.

---

## ◈ AUTONOMOUS AGENT ENGINEERING

ZYRAXON AI focuses on the system surrounding the model: helping transform a user's goal into a workflow that can use tools, observe results, and validate outcomes.

- **Goal-oriented execution** — turn user intent into actionable steps.
- **Tool integration** — connect AI reasoning to external services and execution environments.
- **Multi-agent orchestration** — coordinate specialized agents for larger tasks.
- **Execution and observation** — use tool results to inform subsequent actions.
- **Failure recovery** — handle errors and revise or retry steps where appropriate.
- **Verification** — check results rather than assuming every generated answer means success.
- **Developer extensibility** — support an ecosystem that can evolve through integrations and contributions.

These principles describe the project's engineering direction; consult the source code and release notes to evaluate the implementation in a particular version.

[**Explore the source code →**](https://github.com/onelpawarai-X/ZYRAXON-AI)

---

## ◈ PROJECT ECOSYSTEM

| Resource | Description |
|---|---|
| **ZYRAXON AI** | Main AI agent platform and repository |
| **ZYRAXON Model Provider** | Ten branded model identities through one API interface |
| **MCP Hub** | Model Context Protocol integration work |
| **ZYRAXON Pro** | Pro-oriented platform experience |
| **Agent Ecosystem Hub** | Agent ecosystem and marketplace initiative |

<div align="center">

[Main Platform](https://zyraxonai.lovable.app/) · [Pro Platform](https://zyraxon-pro.ai.studio/) · [Model Provider](https://zyraxonai.lovable.app/providers) · [MCP Hub Source](https://github.com/onelpawarai-X/ZYRAXON-AI/tree/main/MCP%20Hub) · [Agent Ecosystem Hub](https://agent-ecosystem-hub.lovable.app/)

</div>

---

## ◈ GITHUB ENGINEERING METRICS

<div align="center">

<a href="https://github.com/onelpawarai-X">
  <img height="180" src="https://github-readme-stats.vercel.app/api?username=onelpawarai-X&show_icons=true&theme=transparent&hide_border=true&bg_color=050816&title_color=38BDF8&icon_color=8B5CF6&text_color=94A3B8" alt="GitHub statistics"/>
</a>
<a href="https://github.com/onelpawarai-X">
  <img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=onelpawarai-X&layout=compact&theme=transparent&hide_border=true&bg_color=050816&title_color=38BDF8&text_color=94A3B8" alt="Most used languages"/>
</a>

<br/><br/>

<a href="https://github.com/onelpawarai-X">
  <img width="70%" src="https://github-readme-streak-stats.herokuapp.com/?user=onelpawarai-X&theme=transparent&hide_border=true&background=050816&ring=38BDF8&fire=8B5CF6&currStreakLabel=38BDF8" alt="GitHub contribution streak"/>
</a>

</div>

*Metrics are supplied by third-party services and may be affected by caching, availability, or API limits.*

---

## ◈ BUILD WITH US

<div align="center">

### THE NEXT CHAPTER IS BUILT TOGETHER.

**Developers, researchers, designers, testers, and open-source contributors are welcome.**

</div>

Ways to contribute:
- **Code:** improve features, fix bugs, and submit pull requests.
- **Test:** reproduce issues and report clear, actionable feedback.
- **Documentation:** improve setup guides, examples, and API instructions.
- **Integrations:** experiment with tools, models, and compatible workflows.
- **Community:** share demos, tutorials, ideas, and independent reviews.

<div align="center">

<a href="https://github.com/onelpawarai-X/ZYRAXON-AI/blob/main/CONTRIBUTING.md"><img src="https://img.shields.io/badge/CONTRIBUTE-START%20HERE-38BDF8?style=for-the-badge&logo=github&logoColor=FFFFFF" alt="Contribute"/></a>
<a href="https://github.com/onelpawarai-X/ZYRAXON-AI/issues"><img src="https://img.shields.io/badge/ISSUES-FIND%20A%20TASK-8B5CF6?style=for-the-badge&logo=githubissues&logoColor=FFFFFF" alt="Issues"/></a>
<a href="https://github.com/onelpawarai-X/ZYRAXON-AI/discussions"><img src="https://img.shields.io/badge/DISCUSSIONS-JOIN%20IN-A78BFA?style=for-the-badge&logo=github&logoColor=FFFFFF" alt="Discussions"/></a>
<a href="https://www.youtube.com/@ZYRAXONAI"><img src="https://img.shields.io/badge/YOUTUBE-WATCH%20DEMOS-FF0000?style=for-the-badge&logo=youtube&logoColor=FFFFFF" alt="YouTube"/></a>

<br/><br/>

**Explore. Build. Contribute. Improve.**

</div>

---

## ◈ CONNECT

<div align="center">

<a href="https://github.com/onelpawarai-X"><img src="https://img.shields.io/badge/GitHub-Follow%20the%20Journey-181717?style=for-the-badge&logo=github&logoColor=FFFFFF" alt="GitHub"/></a>
<a href="https://www.youtube.com/@ZYRAXONAI"><img src="https://img.shields.io/badge/YouTube-Explore%20Demos-FF0000?style=for-the-badge&logo=youtube&logoColor=FFFFFF" alt="YouTube"/></a>
<a href="https://zyraxonai.lovable.app/"><img src="https://img.shields.io/badge/Platform-Explore%20ZYRAXON-0891B2?style=for-the-badge&logo=openai&logoColor=FFFFFF" alt="Platform"/></a>
<a href="https://zyraxonai.lovable.app/docs/provider-overview"><img src="https://img.shields.io/badge/Developers-Read%20the%20Docs-312E81?style=for-the-badge&logo=readthedocs&logoColor=FFFFFF" alt="Documentation"/></a>

<br/><br/>

### ZYRAXON AI

**Autonomous Agents · Model Infrastructure · Open-Source Engineering**

*Think beyond the prompt. Build beyond the answer.*

<sub>ZYRAXON AI INC. © 2026 · See the repository for the applicable license and terms.</sub>

</div>
'''
