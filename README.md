## Inan Jaggi

AI engineer for operations and supply chain. I spent three internships inside freight, global logistics and manufacturing operations, and now build AI systems for that kind of work. My rule for agents: AI proposes, deterministic code decides, and a person approves anything consequential.

M.S. Information Systems, Indiana University (May 2026). Open to AI forward-deployed engineering roles.

[Website](https://inanjaggi.vercel.app) · [LinkedIn](https://www.linkedin.com/in/inanjaggi) · [Email](mailto:inanjaggi@gmail.com)

### Selected work

Four deployments for one fictional manufacturer, Corvane Industrial, built on synthetic data the way I would run a customer engagement: get the system running, adapt it to the customer's data and policies, evaluate it, and write down what it can't do. Every number traces back to a command in its repo.

| Project | What it does | Result |
| --- | --- | --- |
| [durable-approval-agent](https://github.com/InanJaggi/durable-approval-agent) | LangGraph agent that hands purchase approvals to a Temporal workflow, answered from a chat UI | Exactly one PO after killing the worker mid-approval and mid-write; 26 tests |
| [ap-invoice-matching](https://github.com/InanJaggi/ap-invoice-matching) | Invoice-to-PO and goods-receipt matching on an ERP export, with per-commodity tolerances and exception routing | 52 of 53 invoices correct, 0 false approvals (default settings: 2) |
| [plant-maintenance-agent](https://github.com/InanJaggi/plant-maintenance-agent) | Alarm to diagnosis, parts check, priority and a drafted work order for planner sign-off | 17 of 20 alarms fully correct vs 0 of 20 for the baseline, under 100 ms |
| [spares-forecast-replenishment](https://github.com/InanJaggi/spares-forecast-replenishment) | Weekly forecast-to-order pipeline for 120 SKU-DC series with statsforecast and OR-Tools CP-SAT | 22% lower forecast error; 40% less inventory at a 95% fill rate (simulated) |
| [campus-resource-hub](https://github.com/InanJaggi/campus-resource-hub) | Team capstone I led: Flask booking platform with conflict detection, approvals, waitlist and a Gemini assistant | Team of 4, Kelley School of Business |

[FieldCraft AI](https://inanjaggi.vercel.app/projects/fieldcraft-ai), my governed agentic operations platform, is private. The case study on my site covers how it works and how it's tested.

### How I work

1. **Embed.** Sit with the operators and learn the job as it is done, not as the SOP says.
2. **Prove the value.** Put a dollar figure on the problem from the customer's own data before building.
3. **Build the smallest thing that works.** Reuse what exists, and keep anything that moves money deterministic.
4. **Evaluate and hand off.** Measure against a baseline, gate risky actions behind approval, and leave a runbook.

**Tools:** Python, TypeScript, SQL · LangGraph, Temporal, RAG, MCP · statsforecast, OR-Tools, scikit-learn · FastAPI, Flask, Next.js · Docker, GitHub Actions
