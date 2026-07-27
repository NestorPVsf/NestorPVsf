<p align="center">

  <img src="https://raw.githubusercontent.com/NestorPVsf/NestorPVsf/main/banner.png" alt="Néstor Martínez — AI consultant and engineer" width="100%" />

</p>

<p align="center">

  <img src="https://readme-typing-svg.demolab.com?font=Poppins&weight=600&size=22&duration=3000&pause=800&color=22D3EE&center=true&vCenter=true&width=680&lines=AI+consultant+and+engineer;Agents+that+run+unsupervised+in+production;n8n+automation+and+the+AI+layer+on+top;Full-stack+apps+underneath+(Next.js+%2B+Supabase)" alt="Typing SVG" />

</p>

<p align="center">

<b>One person instead of three suppliers.</b><br/>
I map the process, build the agent, and ship the application it runs on.

</p>



How I work

Process first. I came to this from industrial engineering, an MBA and years in financial consulting. I start from how the business actually works, not from the model.

The AI layer. Agents, retrieval, and the part that takes the time — deciding what the agent isn't allowed to do.

The application underneath. Agents need somewhere to live. I build that too, so there's no coordination tax and no handoffs.

Running in production

Autonomous WhatsApp agent — immigration law firm

11 tools: four retrieve from their legal corpus, three act, four manage its own internal state. It never does arithmetic, because it quotes fees — it calls a whitelisted evaluator instead. Without country, qualification and year, it asks rather than guessing at a legal answer.

A SaaS a business runs entirely from WhatsApp

The owner types an order into a chat. The system issues the invoice, records the expense, updates the CRM and feeds a dashboard. 22 tools, a separate read-only role for their accountant, and EU VAT validated against the official registry rather than a regex.

Consumer assistant, conversations that run for months

No menus, no forms, no flow. A conversation that long outgrows any context window, so memory is tiered: Redis for the live conversation, Postgres for what has to survive it. Answers are retrieved from the corpus rather than packed into the prompt.

What production taught me

An agent will lie to itself across turns if you only persist what it said.

A tool failed silently in one of my systems and the model announced success anyway. That announcement went into conversation history, and on the next turn the model read its own fiction as fact and acted on it. The fix was persisting the tool execution log alongside the assistant message, so the agent's memory holds what happened instead of what it claimed happened.

That failure mode is invisible until it isn't.

Where the code is

Client work lives in private repositories, so this profile is deliberately quiet. Happy to walk through architecture and decisions on a call — usually more useful than a repo tour anyway.

The forks here are tools I use in my own workflow, not projects of mine.

Tech I work with

Elsewhere

🌐 podervsfuerza.com &nbsp;·&nbsp; 💼 LinkedIn &nbsp;·&nbsp; ✉️ info@podervsfuerza.com

<p align="center"><sub>Madrid, working remotely · Available for project and hourly work</sub></p>
