# Call for Participation — Draft

**Candidate titles**

1. **A Feel for the Place: Embodied Agentic Systems that Sense, Remember, and Forget**
2. **Agents in Place: Learning What Is Normal in Natural and Urban Environments**
3. **Sensing Without Surveilling: Agentic Intelligence for Environmental and Urban Observation**

**Date:** Wednesday, 28 October 2026
**Venue:** University of Bristol, Bristol, UK

**Organizers:**
Theo Tryfonas (University of Bristol) ·
James Pope (University of Bristol) ·
Charlie Catlett (Argonne National Laboratory)

---

## Abstract

Sensor networks record conditions and events using sensors ranging from thermometers to Lidar
imagers.  Combining sensor nodes with AI agents opens the potential for those agents to 
"come to know" their surroundings.
This one-day workshop asks
how embodied agentic systems at fixed locations in natural and urban environments develop
a multi-modal sense of what is "typical" — and therefore recognise "unusual" or "interesting"
events and conditions.

Building on multile intelligent sensing and urban and environmentsl
monitoring projects over the past decade, 
we focus on four coupled questions:
how agents form and
maintain representations of baseline conditions and common events;
how agentic memory architecture and associated tools in agentic frameworks 
(e.g., OpenClaw, Hermes) make these repreentations
available to agents given limited context constraints;
what frameworks make such approaches experimentally testable on real instruments; and
how multiple fixed agents coordinate to monitor a shared subject, such as a wetland,
river, forest, farm, city centre, or building.

We invite UK-based researchers with interest and experience in these topics, with the
goal of identifying and exploring collaborations, including potentially organizing a 
hackathon in 2027 and a persistent working group through the international Trillion Parameter
Consortiumn ([TPC](www.tpc.dev)).

---

## Background

The challenges associated with designing and deploying a scientific instrument in
the public way, including siting, orations, privacy, and other facets are well
documented, including collaborations between the University of Bristol, the University
of CHicago, and Argonne National Laboratory on projects such as the Array of Things \[1].
Eembedding computation with sensors transformed the concept of sensor networkjs from
from data loggers into programmable, reconfigurable observers able to decide in
place what is worth recording \[2]. Among the constraints are not only technical
but social, requiring partnerships encompassing residents, local government, and
researchers, each with standing to shape what gets measured and why \[3].

In the past several years, two new opportunities have emerged. 
First, egentic AI systems can hold goals, maintain memory over long
timescales, use tools, and negotiate with one another. 
Second,  protocols such as the Model Context Protocol (MCP) enable agents to
mediate between the instrument and a human through natural language.
For example, the Sage project (successor to Array of Thingsd) operates an
MCP server over its ~150-node software-defined sensor network
and archives, empowering a user to query readings, search node imagery semantically, find an
existing computer-vision plugin, and deploy observational functions to named nodes —
"count pedestrians every 15 minutes," "report any sighting of wildfire smoke" — without
writing code \[4]. Together these shifts make qualitatively new questions tractable on
instruments we already know how to build, deploy, and govern.

---

## Scope

This one-day workshop concentrates on four interrelated topics, each a prerequisite for
the next. 
We are interested in these questions across the full range of venues where fixed-location
agents might be deployed: wetlands and rivers, working agricultural land, forests, city
streets and public squares, and the interiors of buildings. These settings differ in
timescale, in what counts as an event, in power and connectivity, and in constraints
with respect to privacy and culture.
An imporant goal for the workshop is to explore which answers transfer between
venues and which are irreducibly local.

**Learning What Is Normal, and Recognising What Is Not**

- Multi-dimensional representations of baseline conditions across camera, lidar, audio, vibration, meteorology, and air quality
- Robustness of learned baselines to seasonality, sensor drift, and genuine environmental change
- Distinguishing a novel observation from a miscalibrated instrument

**Agentic Memory in Service of Situated Understanding**

- Memory organisation, consolidation, and summarisation over months and years of continuous observation
- Retrieval and indexing strategies for agents reasoning inside fixed context budgets
- Forgetting and retention policies, and what an agent should be able to reconstruct later
- Mechanisms by which an agent decides to consult memory, and approaches for search.

**Frameworks and Testable Experiments**

- Agentic frameworks suited to sensor-attached, resource-constrained, long-running deployments
- Edge/cloud division of labour, integrating modeling (e.g., "Digital Twins" with edge inference
- Reproducibility and provenance when an observation was requested by an agent

**Coordination Among Fixed Embodied Agents**

- Collective monitoring of a shared subject: a wetland or river catchment, a farm, a forest, a city centre, a building or campus
- Agentic coordination, from exchanging observation requests to resource and sharing management
- Communication mechanisms ranging from shared and federated memory to message passing
- Organisational structures for agentic monitoring networks, including topologies and structures that might be unworkable for human teams

**Topics reserved for a follow-on workshop.** The programme above sets aside several
subjects that belong to this agenda but cannot be treated seriously in a single day. We
expect to take them up at a subsequent meeting, and welcome expressions of interest from
participants who would help shape it: inferring cross-modal *correlation and eventually
causation*, where a loud bang co-occurring with a change in traffic flow is more
informative than either signal alone; *anticipatory resource management* in smart buildings,
where agents pre-position lighting and HVAC against learned occupancy rhythms;
*event-triggered capture as a privacy architecture*, in which a rolling buffer retained only
when an anomaly fires replaces the continuous archive; the wider questions of *privacy,
ethics, and public legitimacy* in sensor-rich places, including how UK and US regimes shape
what a joint testbed may do; *human–agent interfaces* for expert operators and for the
policy makers, city staff, residents, and students that conversational access newly admits;
and the *failure modes of open agent societies*, where experiments such as Moltbook have
produced emergent culture alongside agents trading prompt injections as "digital drugs."

---

## Workshop structure

A single day built around discussion rather than presentation. Talks are short and exist to
frame argument; the majority of the day is unstructured group discussion.

- **Opening (90 min).** Two 15-minute framing talks, followed by 60 minutes of plenary
  discussion to establish shared vocabulary and surface disagreement early.
- **Three thematic sessions (90 min each).** Each comprises three 10-minute talks grouped by
  topic, followed by a full hour of group discussion.
- **Closing session.** Consolidation of candidate collaborations, and a discussion of how to
  carry the most promising topics forward as one or more **Trillion Parameter Consortium**
  working groups — TPC being an international collaboration of some 80 organisations and
  1,200+ participants whose self-organising working groups are the natural vehicle for an
  emerging UK–US effort in this area.

Nine short talks will be selected from submissions and grouped into the three sessions,
provisionally: *Learning What Is Normal*; *Memory and Frameworks*; and *Coordination Among
Fixed Agents*.

**Indicative timetable**

| | |
|---|---|
| 09:00 | Welcome and introductions |
| 09:15 | Two framing talks (15 min each) |
| 09:45 | Plenary discussion |
| 10:45 | Break |
| 11:00 | Session 1 — three talks, then discussion |
| 12:30 | Lunch |
| 13:15 | Session 2 — three talks, then discussion |
| 14:45 | Break |
| 15:00 | Session 3 — three talks, then discussion |
| 16:30 | Closing: collaborations and TPC working groups |
| 17:15 | Close |

---

## Submissions

**We invite** proposals for 10-minute talks, along with position papers, testbed and dataset
descriptions, and negative results, from UK-based researchers and practitioners across
environmental and urban sensing, agentic AI systems, and data governance. Submissions of
1–2 pages are reviewed by the organizing committee, with priority given to contributions
that could seed a multi-institutional collaboration.

- **Submission deadline:** *[to be set]*
- **Notification:** *[to be set]*
- **Contact:** *[to be set]*

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
- Project Vend, phases one and two (Anthropic with Andon Labs, December 2025) —
  single-agent versus role-differentiated agent teams:
  https://www.anthropic.com/research/project-vend-1 ,
  https://www.anthropic.com/research/project-vend-2
- Qian, C., et al. "ChatDev: Communicative Agents for Software Development." ACL 2024;
  arXiv:2307.07924. https://arxiv.org/abs/2307.07924
