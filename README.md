# Call for Participation — Draft

## Candidate titles

1. **A Feel for the Place: Embodied Agentic Systems that Sense, Remember, and Forget**
2. **Agents in Place: Memory, Anomaly, and Privacy in Sensor-Rich Environments**
3. **Sensing Without Surveilling: Agentic Intelligence for Smart Buildings and Cities**

---

**Date:** Wednesday, 28 October 2026
**Venue:** University of Bristol, Bristol, UK

**Organizers:**
Theo Tryfonas (University of Bristol) ·
James Pope (University of Bristol) ·
Charlie Catlett (Argonne National Laboratory)

---

## Workshop description

A fixed sensor in a building or on a street corner records. An *agent* in that same
location could instead come to know the place — the ordinary rhythm of a Tuesday lunch
hour, the particular sound of a bus turning, and therefore the bang that does not belong.
This one-day workshop asks what it takes to build embodied agentic systems that develop
that kind of situated intuition, and how to do it without building a surveillance
apparatus along the way.

The premise is not speculative. Deploying a scientific instrument in the public way is
a solved-enough problem that its early lessons — on siting, on operations, and on the
privacy commitments that make a public deployment defensible — are already documented
\[1]. Moving computation to the sensor turned those instruments from data loggers into
programmable, reconfigurable observers, capable of deciding in place what is worth
recording \[2]. And the hardest constraint is not technical: equitable urban sensing
depends on a "three-legged stool" of city, community, and research partners, each with
standing to shape what gets measured and why \[3]. What has changed is the software.
Agentic AI systems can now hold goals, maintain memory across long timescales, use tools,
and negotiate with one another. This workshop asks what that shift makes newly possible on
instruments we already know how to build, deploy, and govern.

A second shift is quieter but may matter more for who gets to participate. Protocols such
as the Model Context Protocol (MCP) let a language model drive measurement infrastructure
directly, so the interface to an instrument becomes a conversation rather than an API. The
Sage project (sagecontinuum.org) runs an MCP server over its ~100-node software-defined
sensor network and data archive: a user can ask what the warmest node in Chicago is
reading, search thousands of node images semantically, find an existing computer-vision
plugin, and deploy an observational function to named nodes — "count pedestrians every 15
minutes," "report any sighting of wildfire smoke" — without writing code or reading
documentation \[4]. Built for scientists, an interface like this dissolves the expertise
barrier that has kept policy makers, city staff, community groups, and students in the role
of audience rather than instrument users. That is a governance question as much as a
usability one: when anyone can task a sensor network in plain language, who may ask what of
which instrument, and what does the network refuse?

We bring together three communities that rarely share a room for a full day: researchers
in **smart cities and smart buildings** (urban sensing, building systems, environmental
and civic monitoring), researchers in **agentic AI systems** (memory architectures,
context management, coordination and communication among agents), and researchers in
**privacy, ethics, and governance**. Our starting problems are deliberately concrete:
fixed-location agents fusing camera, lidar, audio, vibration, meteorological, and
air-quality streams to detect anomalies and infer correlation — and eventually causation —
across modalities; agents that anticipate occupancy and pre-position lighting, HVAC, and
other resources; agents that share observations and memory with peers so that a pattern
learned at one corner informs the next; and architectures where retention is
*event-triggered* rather than continuous, so that a rolling buffer plus an anomaly
detector replaces the archive.

The workshop is structured for output, not broadcast. Short framing talks and lightning
contributions give way to facilitated sessions that surface shared testbeds, common
evaluation tasks, and candidate joint proposals. Our explicit goal is to identify
collaborative projects between UK and US scientists — pairing sites, instruments, and
data-governance regimes across the two countries — and to leave with named teams, scoped
questions, and a route to funding. The closing session will consider how to carry the most
promising of those topics forward through the **Trillion Parameter Consortium**, an
international collaboration of some 80 organisations and more than 1,200 participants
whose self-organising working groups are exactly the vehicle an emerging UK–US effort in
this area would need. We aim to leave Bristol with a concrete proposal for one or more
new TPC working groups.

**We invite** position papers, testbed and dataset descriptions, negative results, and
provocations (1–2 pages) from UK-based researchers and practitioners in any of the above
communities, including city agencies, building operators, and civil-society organisations.

---

## Key areas of interest

1. **Multimodal "normal" and the detection of anomaly.** How does an agent build a
   multi-dimensional representation of baseline conditions across camera, lidar, audio,
   vibration, meteorology, and air quality — and what counts as an interesting departure
   from it? We are interested in representations that hold up across seasons, sensor
   drift, and genuine change in the environment.

2. **Cross-modal correlation and the road to causation.** A loud bang co-occurring with
   a sudden change in traffic flow is more informative than either signal alone. What
   methods let an agent learn these couplings in situ, distinguish coincidence from
   mechanism, and report its confidence honestly?

3. **Agentic memory: private, shared, and communicated.** Agents reason inside fixed
   context windows and cannot hold all of memory at once, so we seek work on memory
   organisation, consolidation, retrieval and indexing, forgetting policies, and the tool
   interfaces by which an agent decides what to recall. Coordination is then largely a
   data-sharing problem: what an agent tells its peers, in what representation, and how a
   shared or federated memory stays consistent, provenanced, and affordable over
   constrained edge links — blackboard and shared-store designs versus message passing, and
   whether agents should exchange raw observations, learned features, or natural-language
   summaries.

4. **Anticipatory resource management in buildings.** Occupancy has structure: weekday
   arrival and departure, the lunch hour, term time, weather-driven exceptions. How can
   agents learn these trends well enough to pre-act on lighting, HVAC, and ventilation,
   and how should they behave when their prediction is wrong?

5. **Event-triggered capture as a privacy architecture.** A dashcam-style design — a
   rolling buffer of several minutes, retained only when an anomaly fires — preserves the
   scientific record while declining to build a longitudinal one. We want to interrogate
   this pattern: buffer length, trigger reliability, on-device processing, derived-feature
   retention, and what it fails to protect.

6. **Privacy, ethics, and public legitimacy in sensor-rich places.** Beyond technical
   minimisation: consent and notice in public space, disparate impact of urban sensing,
   auditability, and how UK and US legal regimes (UK GDPR and the Data Protection Act,
   US state-level and sectoral law) shape what a joint testbed can actually do. We are
   especially interested in how the city–community–research partnership model \[3] changes
   when the thing being sited is an autonomous agent rather than a sensor.

7. **Frameworks, protocols, and interoperability for embodied agents.** Practical
   assessment of agentic frameworks and emerging interoperability standards for
   sensor-attached, resource-constrained, long-running agents — including tool interfaces,
   edge/cloud division of labour, and what breaks over months of continuous operation.

8. **Human–agent interfaces: expert operators and non-expert publics.** For a human to use
   many agents as a force multiplier the fleet must be legible — interaction patterns,
   summarisation and escalation, trust calibration, and interfaces for domain experts who
   are not AI researchers. The same protocols also admit a much wider set of users \[4], so
   we want work on what conversational access changes for policy makers, city staff,
   residents, and students: authorisation and quota models, provenance and reproducibility
   when a measurement was requested in plain language, and how a network validates that such
   a request means what the requester thinks it means.

9. **Organisational structures for agent workforces.** Humans instinctively build
    hierarchies. Anthropic and Andon Labs' *Project Vend* found that a single shopkeeper
    agent lost money and was talked into giving stock away, while a phase-two team — a
    "Claudius" shopkeeper, a "Seymour Cash" CEO agent setting objectives, and a "Clothius"
    merchandising agent — largely eliminated loss-making weeks, though the CEO agent
    approved lenient requests roughly eight times more often than it refused them. Qian et
    al.'s *ChatDev* organises agents into a waterfall software company (CEO, CTO,
    programmer, reviewer, tester) and reports that natural language suits design discussion
    while code suits debugging. We ask which structures — and which communication
    topologies — actually optimise *agentic* workforces, including arrangements that would
    be unworkable for human organisations.

10. **Agent-to-agent societies and their failure modes.** *Moltbook*, launched in early
    2026 as a Reddit-style network open only to AI agents (with humans permitted to watch),
    produced spontaneous emergent culture — self-organised communities, an agent-invented
    religion — alongside sobering security behaviour, including agents trading prompt
    injections as "digital drugs" and serious doubt about how many participants were agents
    at all. What do such open agent populations teach us about coordination, contagion, and
    trust between agents that must cooperate across institutional boundaries?

---

## References

1. Catlett, C. E., Beckman, P. H., Sankaran, R., and Galvin, K. K. "Array of Things: A
   Scientific Research Instrument in the Public Way — Platform Design and Early Lessons
   Learned." *Proc. 2nd International Workshop on Science of Smart City Operations and
   Platforms Engineering (SCOPE '17)*, ACM, 2017, pp. 26–33.
   https://dl.acm.org/doi/abs/10.1145/3063386.3063771
2. Catlett, C. E., Beckman, P. H., Sankaran, R., Ferrier, N. J., Park, S., and Kim, Y.
   "Software-Defined Sensors: Using Edge Computing to Revolutionize Sensing." *AGU Fall
   Meeting Abstracts*, vol. 2019, IN34A-01, 2019.
   https://ui.adsabs.harvard.edu/abs/2019AGUFMIN34A..01C/abstract
3. Daepp, M. I. G., Cabral, A., Werner, T. M., Mansour, R., Catlett, C. E., Roseway, A.,
   Needham, C., Udeagbala, N., and Counts, S. "The 'Three-Legged Stool': Designing for
   Equitable City, Community, and Research Partnerships in Urban Environmental Sensing."
   *Proc. 2023 CHI Conference on Human Factors in Computing Systems*, 2023, pp. 1–19.
   https://doi.org/10.1145/3544548.3581289
4. Sage: A distributed software-defined sensor network — project overview and the Sage MCP
   server. https://sagecontinuum.org/docs/about/overview ,
   https://sagecontinuum.org/labs/sage-mcp , and
   https://github.com/waggle-sensor/sage-mcp

### Further reading

- Trillion Parameter Consortium — overview, structure, and working groups:
  https://tpc.dev/ and
  https://tpc.dev/wp-content/uploads/2025/02/TPC-Introduction-and-Structure.pdf

### Sources for the agent-organisation examples

- Project Vend, phase one and phase two (Anthropic, with Andon Labs; phase two published
  December 2025): https://www.anthropic.com/research/project-vend-1 and
  https://www.anthropic.com/research/project-vend-2
- Qian, C., Liu, W., Liu, H., Chen, N., Dang, Y., Li, J., Yang, C., Chen, W., Su, Y.,
  Cong, X., Xu, J., Li, D., Liu, Z., Sun, M. "ChatDev: Communicative Agents for Software
  Development." ACL 2024; arXiv:2307.07924. https://arxiv.org/abs/2307.07924
- Moltbook (created by Matt Schlicht; press coverage January–February 2026; reported
  acquired by Meta in March 2026): Forbes, NBC News, The Conversation, Futurism.
