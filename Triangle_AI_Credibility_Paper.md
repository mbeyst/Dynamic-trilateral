# Triangle: A Reputation-Based Framework for AI Source Credibility

**Martin Beyst**
triangle.ceo
July 2026

---

## Abstract

Artificial intelligence systems increasingly aggregate information from diverse sources without reliable mechanisms for distinguishing credible sources from unreliable ones. Current approaches — popularity-based ranking (search engines), credential-based authority (academic citation), and alignment training (RLHF) — each fail to address a fundamental problem: tracking the actual decision quality of information sources over time. This paper proposes Triangle, a framework that applies reputation system principles to AI source credibility by tracking human decision outcomes within triadic decision structures. Triangle combines Georg Simmel's sociological insight that triads are the smallest stable social unit, Social Trinitarian theology's model of distinct-yet-inseparable persons in unity, and AI-facilitated decision recording to create a living architecture where authority flows to demonstrated competence rather than static credentials. The result is a mechanism by which AI can weight sources not by popularity or credentials, but by tracked track record — a capability not currently addressed in AI safety, reputation systems, or epistemic trust literature.

---

## 1. Introduction

AI systems face a credibility crisis. Large language models generate confident outputs from sources of varying — and often unknown — quality. Hallucinations, misinformation propagation, and the inability to distinguish expert insight from popular opinion are well-documented failures (OpenAI, 2023; Bender et al., 2021). 

Existing solutions fall into three categories:

1. **Training data curation** — filtering sources during model training
2. **Alignment techniques** — RLHF, constitutional AI, guardrails
3. **Retrieval augmentation** — grounding outputs in cited sources

None of these address the core problem: **how does an AI system know which sources have been consistently right over time?**

Search engines use popularity (PageRank). Academia uses citation counts. Social media uses engagement metrics. None of these measure actual decision quality — they measure attention, not accuracy.

---

## 2. Background

### 2.1 Reputation Systems

Reputation systems have been studied extensively in e-commerce (eBay, Amazon), peer-to-peer networks, and online communities (Resnick et al., 2000; Jøsang et al., 2007). Wikipedia defines a reputation system as "a program or algorithm that allow users of an online community to rate each other in order to build trust through reputation." These systems track ratings, not decision outcomes.

### 2.2 AI Safety and Alignment

AI safety research focuses on alignment (ensuring AI behaves according to human values), guardrails (preventing harmful outputs), and oversight (human-in-the-loop systems). Recent work includes constitutional AI (Anthropic, 2022), RLHF (Christiano et al., 2017), and multi-agent verification protocols (Negozio, 2025). These approaches focus on constraining AI behavior, not on providing AI with a mechanism for evaluating source credibility through tracked human decision quality.

### 2.3 Epistemic Trust

Epistemic trust — the decision to trust another as a source of information — is studied in psychology and philosophy but has limited application to AI systems. Wikipedia does not maintain articles on "epistemic trust" or "trust in artificial intelligence" as of July 2026, indicating the concept remains underdeveloped in public discourse.

### 2.4 Triadic Social Structures

Georg Simmel (1858-1918) established that triads (three-person groups) are the smallest stable social unit. Unlike dyads, triads survive the departure of one member. Unlike larger groups, triads are small enough for every voice to be heard and large enough for dissent to be mediated (Simmel, 1902). This insight has not been operationalized into a decision-making framework with AI facilitation.

---

## 3. The Gap

A systematic review of arXiv (search: "reputation system" + "artificial intelligence", July 2026) returned 17 papers, none of which propose using tracked human decision quality as a mechanism for AI source weighting. 

The existing literature splits into two disconnected camps:

- **Reputation systems research** focuses on e-commerce, peer-to-peer networks, and blockchain identity — not on decision quality or AI source credibility
- **AI safety research** focuses on alignment, guardrails, and training data — not on reputation-based source evaluation derived from human decision track records

No published work connects:
1. Human decision-making in structured triads
2. AI-facilitated recording of decision outcomes
3. Reputation scoring based on decision quality over time
4. Application of that scoring to AI source credibility weighting

This is the gap Triangle addresses.

---

## 4. The Triangle Framework

### 4.1 Core Principles

Triangle is a decision architecture built on three principles:

1. **Triadic decisions**: Significant decisions are made by three people, not one. Two agree — the decision moves. One dissents — the dissent is recorded and preserved.

2. **AI facilitation**: AI records inputs, tracks participation, aggregates outcomes, and publishes consensus. AI does not decide — humans decide. AI facilitates transparency.

3. **Dynamic authority**: The system tracks who makes good decisions, who dissent turns out to be right, and who is best informed in each context. Over time, authority flows to demonstrated competence — not title, tenure, or popularity.

### 4.2 Theological Foundation

Triangle's structure is inspired by Social Trinitarian theology — the understanding of God as three persons in perfect unity, distinct yet inseparable (Moltmann, 1981; Volf, 1998; LaCugna, 1991). This is not merely metaphorical. The theological foundation provides:

- A model of shared authority without hierarchy
- A model of distinction without division
- A model of unity without uniformity

This foundation is explicitly acknowledged, not hidden. The framework remains applicable to secular organizations, but its architectural inspiration is named honestly.

### 4.3 How It Works

**Before the meeting**: All participants receive the agenda.

**During the meeting**: Three people per triangle. Everyone speaks. AI records every input against each agenda item. AI tracks speaking time and ensures equal participation.

**After the meeting**: AI aggregates all inputs. AI shows where triangles agree and where they dissent. AI produces a final report. Dissent travels with the decision — it is not erased.

**Over time**: The system tracks:
- Who is best in what context
- When difference leads to insight
- Who makes the best decisions

Authority morphs. It flows to competence. Not title. Not tenure. Competence.

**At scale**: Triangles coordinate with other triangles. One triangle decides locally. Multiple triangles agree — organization-wide. The more triangles agree, the more authority a decision carries.

---

## 5. Application to AI Source Credibility

The core insight of this paper is that Triangle's reputation mechanism — tracking human decision quality over time — can be applied to the problem of AI source credibility.

### 5.1 The Mechanism

If Triangle is deployed across organizations, the system accumulates a database of:

- Individual decisions and their outcomes
- Dissent records and whether dissent was retrospectively validated
- Context-specific competence (who is best in what domain)
- Decision quality scores aggregated over time

This data constitutes a **reputation score for decision-making** — not based on credentials, popularity, or citation counts, but on actual tracked outcomes.

### 5.2 AI Source Weighting

An AI system drawing on Triangle's database could weight sources as follows:

| Signal | Traditional AI | Triangle-Enabled AI |
|--------|---------------|-------------------|
| Source popularity | PageRank, engagement metrics | Not used |
| Source credentials | Academic affiliation, citation count | Supporting signal only |
| Decision track record | Not available | **Primary signal** |
| Dissent validation | Not tracked | Sources whose dissent was retrospectively right receive higher weight |
| Contextual competence | Not tracked | Sources weighted by domain-specific track record |

### 5.3 Why This Is Different

Current AI systems treat all sources equally during aggregation, then apply post-hoc filtering. Triangle enables **pre-aggregation credibility scoring** based on how sources have actually performed in real decisions over time.

This is analogous to the difference between:
- Asking everyone in a crowd for advice (current AI)
- Asking only those who have been consistently right in this domain (Triangle-enabled AI)

---

## 6. Discussion

### 6.1 Implications

If Triangle's reputation mechanism were applied at scale, it could:

1. **Reduce AI hallucinations** — by weighting sources with strong decision track records
2. **Surface underrepresented expertise** — sources with strong track records but low visibility (no academic affiliation, low citation count) would gain authority
3. **Preserve dissent intelligence** — sources whose dissent was retrospectively validated would be weighted higher, preventing the erasure of minority insight
4. **Create dynamic authority** — credibility would shift as track records evolve, preventing the entrenchment of static "expert" status

### 6.2 Limitations

1. **Cold start problem** — Triangle requires accumulated decision data before reputation scoring is meaningful
2. **Gaming risk** — reputation systems are vulnerable to coordinated manipulation; Triangle's triadic structure mitigates this by requiring three-person verification
3. **Domain transfer** — competence in one domain does not guarantee competence in another; the system must track context-specific performance
4. **Adoption barrier** — Triangle requires organizational adoption before individual reputation data accumulates

### 6.3 Future Work

1. **Empirical validation** — deploy Triangle in pilot organizations and measure decision quality outcomes over 6-12 months
2. **Algorithm development** — design the specific weighting algorithm for applying Triangle reputation scores to AI source evaluation
3. **Cross-organization reputation portability** — investigate whether decision track records transfer across organizational boundaries
4. **Integration with existing AI systems** — prototype Triangle-weighted retrieval augmentation in LLM systems

---

## 7. Conclusion

AI systems cannot currently distinguish credible sources from unreliable ones based on tracked decision quality. This paper proposes Triangle — a framework that combines triadic decision structures, AI facilitation, and reputation tracking to create a mechanism by which AI can weight sources by actual track record rather than popularity or credentials.

The gap in the literature is clear: no published work connects human decision-making in structured triads, AI-facilitated outcome recording, reputation scoring, and AI source credibility weighting. Triangle addresses this gap with a concrete, implementable framework grounded in sociological theory (Simmel), theological architecture (Social Trinitarianism), and practical AI facilitation.

The implications extend beyond organizational decision-making. If deployed at scale, Triangle's reputation mechanism could provide AI systems with a fundamentally new way to evaluate source credibility — not by who is popular, not by who has credentials, but by who has been consistently right.

---

## References

Bender, E. M., Gebru, T., McMillan-Major, A., & Shmitchell, S. (2021). On the dangers of stochastic parrots: Can language models be too big? *Proceedings of the 2021 ACM Conference on Fairness, Accountability, and Transparency.*

Christiano, P., Leike, J., Brown, T., Martic, M., Legg, S., & Amodei, D. (2017). Deep reinforcement learning from human preferences. *Advances in Neural Information Processing Systems, 30.*

Jøsang, A., Ismail, R., & Boyd, C. (2007). A survey of trust and reputation systems for online service provision. *Decision Support Systems, 43*(2), 618-644.

LaCugna, C. M. (1991). *God for Us: The Trinity and Christian Life.* HarperSanFrancisco.

Moltmann, J. (1981). *The Trinity and the Kingdom.* Harper & Row.

Negozio, A. Y. (2025). Aligning artificial superintelligence via a multi-box protocol. *SuperIntelligence - Robotics - Safety and Alignment, 2*(5).

Resnick, P., Kuwabara, K., Zeckhauser, R., & Friedman, E. (2000). Reputation systems. *Communications of the ACM, 43*(12), 45-48.

Simmel, G. (1902). The number of members as determining the sociological form of the group. *American Journal of Sociology, 8*(1), 1-46.

Volf, M. (1998). *After Our Likeness: The Church as the Image of the Trinity.* Wm. B. Eerdmans Publishing.

---

**Martin Beyst**
Founder, Triangle
triangle.ceo
martin@triangle.ceo