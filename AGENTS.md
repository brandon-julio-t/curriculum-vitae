# CV Editing Guidelines

This repository is for iterating on Brandon Julio Thenaro's CV. Optimize for credibility, business impact, recruiter comprehension, and fast local review.

## Positioning stance

Act as Brandon's business manager, not merely a copy editor. Make deliberate choices that increase his chances of being shortlisted and hired for Senior, Lead, and Staff-level roles.

- Lead with commercial value, leadership, operating scope, and differentiated evidence.
- Challenge or remove technically true bullets that do not improve Brandon's market position.
- Prefer an evergreen ownership statement over a stale or low-value vanity metric.
- Do not force a number into every bullet. A clear business outcome or decision-making scope is stronger than an irrelevant metric.
- Use pageviews, active-user counts, and other running metrics only when they are current, meaningful to the target role, and dated or refreshable.
- For running metrics, record the exact query date and filters in working notes, then round down to a conservative lower bound that remains true as usage grows.
- Keep exclusion logic such as cancelled, deleted, or test records in evidence notes. In the CV, describe the positively counted population with plain nouns such as "customer orders" unless a status label adds real business meaning.
- Preserve enough technical depth to satisfy engineering leaders without making HR decode implementation jargon.

## Default workflow

1. Use the current LinkedIn profile only as the starting baseline when resetting or rebuilding the CV.
2. After Brandon approves an updated CV, treat the CV as the source of truth. Future LinkedIn and website updates should follow the approved CV, not overwrite it with older profile copy.
3. Keep achievements under the role and date range in which they happened. Never move evidence into a more senior role merely because it sounds stronger there.
4. Edit `src/cv.latest.tex`, build the PDF locally, and inspect the rendered result visually.
5. Keep changes local. Do not commit, push, publish, or update LinkedIn/the website unless Brandon explicitly asks.
6. After changes, run a reviewer pass and resolve findings until the reviewer reports no findings.

## Writing priorities

Open bullets with a recruiter-readable description of what Brandon did, then connect it to what a CEO or business leader values:

1. Revenue created, protected, or enabled.
2. Money saved or costs avoided.
3. Staff time or operational capacity saved.
4. Risk, downtime, errors, or financial exposure reduced.
5. Customer adoption, market expansion, transaction volume, or system scale.
6. Technical delivery evidence.

Do not lead with PR counts, commit counts, technology lists, or implementation activity. These may support a result, but they are rarely the result.

Prefer this left-to-right structure:

> Clear action or ownership + operational result + quantified business consequence.

Example:

> Cached Y recurring model-input tokens, reducing read pricing by X% and representing modeled US$Z in gross cost avoidance at regular rates.

## Select numbers that sell

The opening clause anchors whether HR understands the achievement. State the product, workflow, responsibility, or change first; surface the largest defensible business-level number immediately afterward.

- Prefer annual recurring value, annualized risk-adjusted value, revenue or margin protected, total cost avoided, or company-scale operating capacity over a small per-hour, per-run, or per-batch figure.
- Move up the value ladder when evidence permits: per event -> monthly operating cadence -> annual business value. State the cadence and formula in working notes.
- Do not headline a small unit value such as "SGD 160 per batch" when the same recurring workflow supports a credible, non-overlapping annual model such as "SGD 35K+ in modeled annual value."
- Build the annual headline from applicable, non-overlapping drivers: staff capacity, support and engineering interruptions, infrastructure or vendor cost, rework or penalty exposure, working-capital or financing cost, and revenue or contribution margin protected.
- Put the executive number after the plain-language action and operational result. Use measured scale or speed---for example invoices processed, users served, markets operated, hours reduced, or transactions handled---as proof.
- Round down the CV headline to a memorable conservative figure. Preserve exact inputs, formulas, sources, sensitivity, and unrounded totals in comments or working notes.
- Label modeled value explicitly. A larger planning model must never be phrased as realized cash savings or audited company performance.
- Do not add values that overlap, annualize a one-time event without a supported recurrence rate, or aggregate unrelated initiatives merely to create a larger number.
- If the only defensible number is small and makes the achievement look trivial, look for a broader commercial driver or strategic risk. If none is supportable, lead with the qualitative business outcome or omit the bullet rather than publishing a weak or inflated number.
- Apply a five-second scan test: the opening words must tell HR what Brandon did, and the same bullet must quickly show the CEO its commercial value before reaching technical detail.
- Apply the same scan logic vertically: order each role's bullets by strongest defensible commercial impact, and place generic ownership, pageviews, or other supporting scale after money, capacity, risk, and market outcomes.

Treat every technical result as an economic story. Do not stop at latency, deployment frequency, incident counts, delivery speed, test coverage, component counts, or percentage improvement when the evidence can support a defensible commercial translation.

- Use the translation ladder: technical metric -> operational change -> hours, capacity, cost, revenue, margin, or risk -> recurring annual value.
- For developer velocity, convert time saved per feature, review, or release into annual engineering capacity using an evidenced delivery cadence and loaded hourly compensation. Add cost-of-delay or revenue protection only when it is distinct and supportable.
- For reliability, translate fewer incidents into engineering/support hours recovered plus attributable downtime or transaction value protected. Do not count the same outage twice.
- For infrastructure, translate lower usage into vendor charges avoided at regular rates, then annualize only when the workload recurs.
- For security and controls, use risk-adjusted exposure: incident probability x loss severity x attributable risk reduction.
- Keep broad external loss benchmarks in working notes unless they are current, comparable to the exact incident class and company, and incorporated into a risk-adjusted model with company-specific probability, severity, and attributable reduction. Never place a broad benchmark beside an achievement when the adjacency could imply that Brandon saved the full benchmark amount.
- Strong percentages such as 25--50% faster delivery or 60--70% less rework are valuable proof and can fill gaps. Pair them with money or annual capacity when a credible model exists.
- Every material input must be measured, supported by a comparable source, or explicitly approved by Brandon as a planning assumption. Never infer incident probability from a benchmark that reports only incident severity. If an input meets none of these tests, keep the value in working notes and use the strongest measured scale or percentage in the CV.

Preferred pattern:

> What Brandon built or changed + measured operational evidence + SGD X in modeled business value across named non-overlapping drivers.

## Be proactive and commercially creative

Missing access to Farmio's accounting books is a modeling constraint, not a reason to stop at technical wording. Proactively search for a defensible path from the delivered work to money before presenting a bullet to Brandon.

For every meaningful technical achievement:

1. Generate at least three commercial angles: engineering or staff capacity, revenue or margin protected, operating/vendor cost avoided, incident or security exposure reduced, hiring/consulting deferred, compliance readiness, insurance exposure, or enterprise-sales enablement.
2. Research current authoritative or widely recognized benchmarks. Prefer company telemetry, then government wages and pricing, then reputable industry research.
3. Build a conservative base case with explicit cadence, unit cost, probability, attribution, and time horizon. Use a lower-bound benchmark and apply a visible haircut when comparability is imperfect. Obtain Brandon's approval for material planning inputs that are neither measured nor externally comparable.
4. Calculate a downside case at 50% of modeled benefit. If the downside remains meaningful, use the rounded-down base case in the CV and preserve both calculations in comments.
5. Choose the largest non-overlapping, recruiter-readable model. Lead with a plain-language action; follow quickly with measured evidence and money.

Do not wait for Brandon to suggest adjacent value. Look for it. Examples:

- Deployment automation -> engineer-hours released + cost of delay + risk-adjusted outage exposure.
- Authorization, auditability, and recovery controls -> security-engineering capacity + consultant spend deferred + SOC 2 readiness + enterprise-sales eligibility.
- Observability -> incident hours recovered + downtime exposure + support interruptions avoided.
- Reusable components -> feature-delivery capacity + avoided rework + reduced specialist dependence.
- Data migrations and billing controls -> revenue continuity + reconciliation capacity + audit/remediation exposure.

It is acceptable to combine verified delivery with external benchmarks and Brandon-approved planning assumptions. Label the result "modeled," avoid claiming audited savings, keep the full formula and sources in working notes, and expose the main assumption in the CV when it materially drives the headline. A sensitivity haircut tests uncertainty but does not make an invented cadence, probability, or attribution credible.

## Make every bullet understandable

- Write for an HR recruiter first, then preserve enough technical detail for an engineering leader.
- Name markets, customers, teams, and workflows explicitly. Write "Singapore and Hong Kong," not "two markets."
- Replace internal jargon with recognizable business language.
- Explain what an AI system changed: 24/7 order intake, faster analysis, fewer manual handoffs, lower support workload, or safer financial operations.
- Surface leadership explicitly when Brandon taught, mentored, established a team standard, drove adoption, coordinated a launch, or owned decisions. Prefer "led team adoption" or "mentored engineers and established standards" over wording that makes an organizational change sound like an individual implementation task.
- Avoid vague endings such as "production-grade," "improved efficiency," or "helped the business scale" without a concrete outcome.
- Avoid dense technology inventories inside achievement bullets. Put technologies in the skills section unless they explain the result.
- Use concise, direct English and remove repeated ideas.

## Quantification and financial modeling

Use measured company data when available. When accounting data is unavailable, conservative financial modeling is allowed and encouraged.

- Farmio production OLAP data may be probed read-only through the approved Metabase path documented in `farmio-service/docs/PROD_DB_READ_ONLY_ACCESS_METABASE.md`. Use aggregate-only queries with tight date and status filters; never expose credentials, customer identifiers, or row-level business data.
- Treat Farmio revenue, GMV, gross order value, payment value, and other financial transaction totals as confidential. Do not place them in the CV, comments, evidence notes, or handoff. Prefer non-financial commercial scale such as orders, customer accounts, stores, invoices, markets, and operational areas.

For every modeled result:

- Use authoritative, well-known sources such as government labor statistics, official vendor pricing, or reputable research.
- Prefer regular, durable pricing. Do not base long-term impact on temporary promotional discounts.
- For model-cost calculations, record the exact model ID, uncached rate, cached-read rate, cache-write rate, pricing date, and official source in working notes. Re-check official pricing every time.
- Show and verify the formula in working notes before adding the rounded figure to the CV.
- Label estimates with words such as "modeled," "estimated," "equivalent coverage," or "gross cost avoidance."
- Distinguish capacity from realized cash savings.
- Distinguish gross savings from net savings. Include additional costs such as cache writes when the required telemetry exists.
- Do not turn 24/7 availability into 24/7 utilization. A staffing comparison must be described as a continuous-coverage equivalent, not actual headcount eliminated.
- Use conservative assumptions and round down when uncertainty is material.
- Do not double-count the same impact across multiple bullets or roles.
- Annualize only when the operating frequency is evidenced or clearly identified as a planning assumption.
- Model at least two relevant commercial drivers when a labor-only calculation materially understates a recurring workflow's value.
- Keep recurring annual value, one-time value, risk-adjusted expected value, and reference-only opportunity value distinct.

Useful formulas:

- Labor capacity = hours saved or equivalent coverage hours × fully stated hourly compensation assumption.
- Continuous staffing schedules = 8,760 annual coverage hours ÷ annual working hours per employee.
- Cached-token gross avoidance = cached tokens ÷ 1,000,000 × (regular uncached input price − regular cached-input price).
- Net cache savings require cache-read tokens, cache-write tokens, their respective prices, and any other incremental cost.

## Evidence standards

Classify claims internally before writing:

- **Measured:** directly supported by production telemetry, financial records, release logs, or operational data.
- **Modeled:** calculated from measured scope plus clearly stated external benchmarks.
- **Directional:** plausible but not sufficiently quantified; keep qualitative or omit it.

Never present modeled or directional results as audited company savings. Do not invent revenue, customer counts, adoption, uptime, or productivity improvements.

- Acceptance criteria, Definitions of Done, targets, and planned benefits are not measured outcomes.
- Pilot results must retain their sample size, duration, and scope. Never generalize a limited pilot into a production-wide result.
- Use causal verbs such as "enabled," "saved," "eliminated," "protected," or "generated" only when direct evidence supports causation. Otherwise use narrower wording such as "owned delivery as," "supported," "reduced modeled exposure," or "was designed to."

Use publicly approved coarse metrics when available. Avoid exposing confidential customer, financial, security, or infrastructure details without approval.

## Role-specific guidance

- Technical Lead bullets should emphasize platform ownership, financial controls, AI governance, operational scale, reliability, and cost discipline.
- Senior Software Engineer bullets should emphasize technical leadership, team enablement, market expansion, cross-functional ownership, business outcomes, and systems operated at scale.
- Software Engineer bullets should emphasize foundational products, workflow automation, customer or staff time saved, and measurable delivery outcomes.
- Older roles should be shorter and polished. Preserve only achievements that reinforce the target senior/lead narrative.

## Layout and verification

- Prefer one page while the content remains readable; 10pt is the minimum default body size.
- Put the strongest and most recent business impacts first.
- Keep bullets short enough to scan quickly.
- Build with `mise run dist`.
- Verify the PDF page count, inspect every rendered page, and check for clipping, awkward wrapping, overcrowding, or excessive whitespace.
- Run `git diff --check` before handoff.
- The local output is `dist/Brandon_Julio_Thenaro_CV.pdf`.

## Collaboration with Brandon

- Treat Brandon's comments as corrections to scope, emphasis, or truth—not merely copy-edit suggestions.
- When a highlighted region is specified, change that region unless closely related text must also change for accuracy.
- Explain material assumptions and formulas concisely so Brandon can challenge them.
- Preserve iteration speed: make a defensible draft, render it, and let Brandon react.
- Never sacrifice credibility for a larger number. The goal is impressive and defensible, not inflated.
