# Portable Modules — Plain-Language Guide

**Project:** The Concord  
**Purpose:** A non-technical front door to the graduated portable modules  
**Status:** Living guide — expand as additional modules graduate  
**Date:** September 2026

## Why this guide exists

The portable modules are intended to be reusable outside the Concord, but their formal names and specifications can make them look more specialised or technical than the underlying ideas actually are.

This guide answers a simpler question:

> **What does this tool actually help me do?**

It does not replace the formal specifications. The examples below are deliberately simple illustrations. They show the kind of problem a module addresses; they do not prove that the module has been empirically validated in every listed domain.

For rigorous application, use the corresponding portable-module specification.

---

# 1. Reality Trees

## Plain-English name

**Map the realistic possibilities before choosing one.**

## What does it do?

Reality Trees help you lay out several possible explanations, choices, outcomes or pathways without prematurely deciding that one must be correct.

Instead of thinking:

> “It must be A.”

you deliberately ask:

> “Could it be A, B, C or something we have not considered yet? What evidence and assumptions belong to each possibility?”

Branches can then be examined, tested, weakened, strengthened, deferred or rejected as new information appears.

## Simple example

Your car will not start.

One possibility is a flat battery. Another is that there is no fuel. Another is a starter-motor problem.

Rather than immediately buying a new battery because that was your first idea, you make the alternatives explicit and check what evidence would distinguish them.

A failed branch is still useful: discovering that the battery is healthy removes one explanation and improves the remaining search.

## Where could it be applied?

Potential applications include everyday decisions, troubleshooting, diagnosis, research, engineering, planning, strategy, investigation, design, risk analysis, AI reasoning and situations where personal belief and available evidence point in different directions.

## Use it when

Use a Reality Tree when there are several materially different possibilities and choosing one too early could hide a better explanation or pathway.

## What it does not do

A Reality Tree does not prove that a branch is true. Showing a possibility does not make it equally likely to every other possibility, and a confidence weight is not automatically a mathematical probability.

**Formal module:** *Reality Trees — A Portable Method for Weighted Possibility-Space Reasoning*

---

# 2. Functionally Bounded Summits

## Plain-English name

**Solve the problem you actually came to solve without dragging every other dispute into it.**

## What does it do?

Functionally Bounded Summits provide a way for people, organisations or systems that disagree about many things to cooperate on one specific problem.

The basic idea is:

> **Bound the problem. Bound the negotiation. Bound the failure. Expand only when the problem genuinely requires it.**

Participants do not have to become friends, settle every disagreement or agree on a common worldview before solving the limited problem in front of them.

## Simple example

Two neighbours have argued for years about noise, parking and a boundary fence. A tree then falls across both driveways.

A functionally bounded discussion can address:

> “How do we remove this tree?”

without requiring either neighbour to settle the fence dispute, apologise for every previous argument or renegotiate their entire relationship.

If removing the tree genuinely requires access across the disputed boundary, that dependency can be brought into scope deliberately.

## Where could it be applied?

Potential applications include workplace disputes, business negotiations, communities, institutions, technical standards groups, federated systems, multi-agent systems, jurisdictions and other situations where limited cooperation is possible despite wider disagreement.

## Use it when

Use it when a practical problem may be separable from a much larger contested relationship and allowing every surrounding dispute into the negotiation could prevent useful cooperation.

## What it does not do

It does not pretend wider disagreements have disappeared. It also must not artificially exclude something that the bounded problem genuinely depends upon.

**Formal module:** *Functionally Bounded Summits — A Portable Protocol for Bounded Negotiation and Failure Containment*

---

# 3. Blaineyan Reasoning

## Plain-English name

**Explore a difficult problem from more than one angle, including the possibility that you are asking the wrong question.**

## What does it do?

Blaineyan Reasoning is an exploratory reasoning method for complex or poorly defined problems.

Its operating cycle can move through:

**Observe → Compare → Abstract → Ground → Speculate → Branch → Examine → Prune → Reconsider → Re-ground → Refine**

The important feature is that the initial framing of the problem is not treated as untouchable. If exploration reveals that the question, boundary or abstraction level is wrong, the method allows you to move back and reformulate it.

It permits speculation, but keeps speculation separate from evidence.

## Simple example

A shop asks:

> “How do we make the checkout queue move faster?”

A narrow answer might be “hire another cashier.”

Blaineyan Reasoning allows the problem to be reconsidered. Perhaps the real issue is not cashier speed at all. Customers may be waiting because price labels are unclear, payment equipment is unreliable, or everyone arrives during one short period.

The method explores these possibilities, checks them against reality, rejects weak branches and returns promising explanations or designs to appropriate specialist methods for testing.

## Where could it be applied?

Potential applications include research, engineering, system design, strategy, invention, organisational problems, policy analysis, AI reasoning and other complex questions with uncertain boundaries or incomplete possibility spaces.

## Use it when

Use it when a problem is complex, interacting, poorly framed or resistant to obvious solutions—especially when you suspect the apparent question may not be the underlying question.

## What it does not do

It does not replace scientific testing, engineering verification, legal analysis or other specialist methods. Speculating about a possibility is not evidence that it is true.

Reality Trees can be used within Blaineyan Reasoning, but Reality Trees are a separate method and are not required.

**Formal module:** *Blaineyan Reasoning — Portable Module*

---

# 4. Minimum Necessary Capability

## Plain-English name

**Give someone enough power to do the job, but not more power than the job actually needs.**

## What does it do?

Minimum Necessary Capability (MNC) helps determine how much access, authority, permission or practical capability is justified by a legitimate function.

It guards against two opposite mistakes:

- giving too much capability; and
- giving so little capability that the assigned job cannot actually be done.

Its basic chain is:

**Purpose → Function → Need → Minimum Sufficient Capability → Bounded Exercise → Review → Termination or Re-Justification**

So “minimum necessary” does not mean “as little as physically possible.” It means the least capability that is still sufficient for the legitimate function.

## Simple example

A plumber needs to repair a leaking pipe in your house.

The plumber may need access to the house, the affected room and the water shut-off.

That does not mean the plumber needs permanent access to your house, your computer, your bank account or every locked room.

But giving the plumber permission to look at the pipe while refusing access to the shut-off valve might also make the repair impossible.

MNC asks what capability is actually required, what would be excessive, how long it should last and when it should end.

## Where could it be applied?

Potential applications include software permissions, AI-agent tool access, employee roles, contractor access, data permissions, delegated authority, infrastructure administration, physical access, emergency powers and other situations where one actor can materially affect another person, resource or system.

## Use it when

Use MNC when somebody or something needs consequential capability in order to perform a legitimate function and you need to determine appropriate limits.

## What it does not do

MNC does not decide whether the underlying purpose is legitimate. That legitimacy must come from the applicable legal, contractual, organisational, consensual or other legitimate framework.

It also does not mean that logging an action makes an otherwise unjustified action legitimate.

**Formal module:** *Minimum Necessary Capability — A Portable Architecture for Bounding Power, Permission and Access*

---

# 5. Contextual Wrapper Architecture

## Plain-English name

**Make it clear when you enter a place or situation where the rules are different—and exactly what those differences mean.**

## What does it do?

Contextual Wrapper Architecture (CWA) handles bounded situations where rules, permissions, risks, roles or expectations legitimately differ from the surrounding environment.

Its principle is:

> **Standardise the interface; preserve legitimate contextual variation.**

The aim is not to make every environment obey identical rules. It is to make the change of context understandable: where it begins, what changes, what does not change, who has relevant responsibility or authority, how someone exits, what happens in an emergency and when the special context ends.

## Simple example

A boxing match allows actions that would normally be unacceptable between two people outside the ring.

But stepping into the ring does not mean:

> “Anything whatsoever is now permitted.”

There are still boundaries, rules, consent conditions, officials, stopping conditions and emergency procedures.

The boxing ring is therefore a simple example of a bounded context: some conditions change inside it, while other protections remain.

## Where could it be applied?

Potential applications include sports, laboratories, workplaces, medical settings, private or restricted spaces, websites, online communities, games, temporary events, transport systems, institutions, special jurisdictions and mixed physical/digital environments.

## Use it when

Use CWA when entering or creating a bounded context materially changes rules, permissions, restrictions, roles, risks, responsibilities or expectations.

## What it does not do

CWA does not decide what every context's rules should be, and it does not mean entering a context automatically constitutes unlimited consent.

It standardises how contextual difference is represented and managed more strongly than it standardises the substantive outcome.

**Formal module:** *Contextual Wrapper Architecture — A Portable Architecture for Bounded Contexts*

---

# 6. Architectural Unit Resolution

## Plain-English name

**Before saying something is missing from a system, check whether you are looking in the right part of the system.**

## What does it do?

Architectural Unit Resolution (AUR) helps prevent two opposite errors:

1. declaring that a system is missing something merely because one component does not contain it; and
2. assuming that something is adequately handled elsewhere merely because another component is mentioned.

Its simplest principle is:

> **Document ≠ necessarily System**

AUR asks what the component is actually responsible for, what neighbouring components legitimately belong to the relevant system family, whether the missing function belongs elsewhere, and whether the connection to that external function actually works.

## Simple example

You inspect a restaurant kitchen and notice that it contains no cash register.

It would be a mistake to conclude:

> “This restaurant has forgotten how to take payment.”

Payment may correctly be handled at the front counter.

But it would also be a mistake to accept:

> “Payments are handled somewhere else.”

without checking whether a payment system actually exists and connects properly to the restaurant's operation.

AUR distinguishes a legitimate division of responsibilities from a genuine missing function or a broken connection between components.

## Where could it be applied?

Potential applications include software architecture, organisations, businesses, engineering systems, research frameworks, AI systems, institutional design, documentation sets and other systems made from multiple connected parts.

## Use it when

Use AUR when someone argues:

> “This component doesn't contain X, therefore the system is missing X.”

or:

> “Another component handles X, therefore there is no problem.”

AUR tests both claims.

## What it does not do

AUR does not redesign the system or decide what should be built next. It diagnoses where a function belongs, whether it exists and whether the relevant interfaces are adequate.

Finding no mechanism within the bounded search also does not prove that no mechanism exists anywhere.

**Formal module:** *Architectural Unit Resolution — A Portable Method for Resolving Architectural Units Before Gap Classification*

---

# 7. Continuity Protocol

## Plain-English name

**Preserve what matters so it can still work after change, loss or replacement.**

## What does it do?

The Continuity Protocol helps distinguish merely keeping copies from preserving enough knowledge, capability and dependencies to recover a valuable function.

Its core idea is:

> **Preserve what remains valuable; adapt what must change; retain enough knowledge, provenance and enabling capability to recover legitimate function after disruption.**

It asks what actually needs to continue, what may legitimately change, what disruption is being planned for, what dependencies recovery requires, how quickly recovery must happen, how much recent state may be lost, and how recovery will be verified.

## Simple example

A business backs up its customer database every night.

The backup exists, so the data is recorded. But after a fire the business discovers that the backup requires obsolete software, the decryption key was stored in the destroyed building, and nobody has tested a restoration for years.

The business had copies, but it did not have a complete recovery basis.

The Continuity Protocol would have asked whether the backup was accessible, interpretable, actionable and genuinely recoverable—and what other dependencies had to survive with it.

## Where could it be applied?

Potential applications include organisations, software and digital services, engineering systems, research programmes, archives, infrastructure, succession planning, emergency recovery, long-duration projects, institutional knowledge, AI systems and other situations where valuable function must survive change or disruption.

## Use it when

Use the Continuity Protocol when something important must survive staff turnover, technical replacement, failure, disaster, institutional change or another discontinuity—and merely saying “we have a backup” is not enough.

## What it does not do

The protocol does not require the current implementation to survive forever. Preserving a function may legitimately involve replacing the original system.

It also does not create legal authority, establish ethical legitimacy, guarantee recovery under every possible disruption or prove that every dependency has been discovered.

**Formal module:** *Continuity Protocol — Portable Module*

---

# 8. Cross Boundary Externality Recognition

## Plain-English name

**Notice when your actions affect someone outside your boundary—without assuming that gives either side unlimited authority over the other.**

## What does it do?

Cross Boundary Externality Recognition helps represent consequences that pass from one organisation, system, community or other bounded domain into another.

Its simplest principle is:

> **Make the consequence legible; keep responsibility, authority and remedy separate.**

A consequence can be real even when the parties do not share a government, contract, regulator or decision process. But recognising that consequence does not automatically prove who caused it, who is responsible, who has authority to act or what remedy is legitimate.

## Simple example

A farm changes how it uses fertiliser. Later, a downstream reservoir detects elevated nitrate levels.

That is enough to investigate whether a cross-boundary consequence exists.

It is not enough by itself to conclude:

> “The farm caused everything downstream, so the reservoir operator may now control how the farm operates.”

Rainfall, seasonal changes or other tributaries may also contribute. The reservoir operator may have authority to monitor or manage its own water system without having authority over the farm.

The module keeps those questions separate while allowing evidence, voluntary mitigation and legitimate response pathways to develop.

## Where could it be applied?

Potential applications include environmental effects, shared infrastructure, digital networks, supply chains, organisations, communities, federated systems, resource management, cross-jurisdictional problems and other situations where consequences cross boundaries that authority does not automatically cross.

## Use it when

Use it when one bounded actor, system or condition may materially affect another domain and the affected parties do not share a simple or uncontested authority structure.

It is particularly useful when causation is uncertain, responsibility may be distributed, parties disagree about standing or authority, or some useful response is possible without resolving the entire relationship.

## What it does not do

The module does not turn an allegation into proof, a consequence into automatic responsibility, responsibility into jurisdiction, or jurisdiction into unlimited authority.

It does not calculate legal or financial liability, determine universal standing, impose compensation or manufacture a shared government.

**Formal module:** *Cross Boundary Externality Recognition — Portable Module*

---

# How the modules differ

Several modules may appear applicable to the same problem because they operate at different layers.

**Reality Trees** asks: *What are the materially different possibilities?*

**Blaineyan Reasoning** asks: *Are we exploring the problem broadly enough, at the right level and with the right framing?*

**Architectural Unit Resolution** asks: *Are we evaluating the correct part of the system before declaring a gap?*

**Minimum Necessary Capability** asks: *How much capability is actually justified by the required function?*

**Contextual Wrapper Architecture** asks: *How should materially different conditions inside a bounded context be made clear and managed?*

**Functionally Bounded Summits** asks: *Can we cooperate on this particular problem without turning it into a negotiation over everything else?*

**Continuity Protocol** asks: *What must survive a disruption, and have we preserved enough to make the required function genuinely recoverable?*

**Cross Boundary Externality Recognition** asks: *What consequence crossed a boundary, what does the evidence support, and what response is legitimate without manufacturing authority?*

They are therefore not competing solutions to one problem. They are reusable tools for different recurring problem structures.

---

# Future organisation

This guide deliberately does **not** yet assign the modules to fixed domains.

Many portable modules are intentionally cross-domain. Premature classification could make a general method appear to belong only to AI, governance, research, software or another particular field.

As additional modules graduate, this guide should be extended using the same plain-language structure.

When the portable-module set is substantially complete, a second navigation layer should be developed around questions such as:

> **“I have this kind of problem — which module might help?”**

At that stage modules can also be indexed by relevant application domains without treating those domains as exclusive boundaries.

---

## Evidential note

“Graduated” in this guide means the module has completed the Concord's portable-development and bounded transfer-testing process at specification level.

It does not mean that the module has been universally or empirically validated in every candidate application listed above.
