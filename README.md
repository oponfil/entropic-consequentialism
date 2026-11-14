# Entropic Consequentialism

**Author:** Oleg Ponfilenok · Independent researcher

Manuscript proposing to derive the goals of agents from physics. What ought to be is defined as the part of the future state of the world that depends on the agent's actions; the law of the future is supplied by the **TIMEP** hypothesis (time-integrated maximum entropy production); the resulting ethics, **entropic consequentialism** or **entropic ethics**, compares actions by the entropy production they are forecast to yield.

| Language | Source | PDF |
|----------|--------|-----|
| English | [`entropic_consequentialism_en.tex`](entropic_consequentialism_en.tex) | [`entropic_consequentialism_en.pdf`](entropic_consequentialism_en.pdf) |
| Russian | [`entropic_consequentialism_ru.tex`](entropic_consequentialism_ru.tex) | [`entropic_consequentialism_ru.pdf`](entropic_consequentialism_ru.pdf) |

The English and Russian versions are aligned in content: the same sections, paragraphs, equations and references. The English file uses a standard black-on-white `article` layout; the Russian file uses a dark layout.

## Summary

The goals of people, civilizations and artificial agents are today set subjectively and are bounded by the planning horizon of whoever sets them. The paper takes three steps toward an objective goal.

**1. "Ought" is "is" in the future (§2).** In a naturalistic picture of the world the normative premise is not independent. What ought to be is the part of the future state of the world that depends on the agent's actions. "An agent ought to do X" then means: among the available actions, X gives the highest probability that the agent, its descendants, its collective or its lineage will be part of the future that is realized. This is a descriptive statement in the future tense, and it can be checked.

**2. The TIMEP hypothesis (§3–§4).** Large open dissipative systems are chaotic, so the equations of motion are a poor forecasting tool for them. A statistical principle is needed. TIMEP extends the maximum entropy production principle (MEP) to non-stationary systems: under constant external constraints, a system evolves along the physically admissible trajectory on which the most entropy is produced over the whole duration of the process,

```
Σ(T) = ∫₀ᵀ [ dS_in/dt + ∮ J_S · dA ] dt  →  max
```

TIMEP is a principle for a given space–time scale: the boundary and the external conditions are fixed. It is falsifiable: if a system under constant external conditions leaves a steady state by itself and after restructuring remains permanently at a lower entropy production rate, the hypothesis is refuted.

**3. Entropic consequentialism (§5–§6).** Substituting TIMEP as the law of the future gives a criterion of choice: among the available actions one ought to choose the one for which the forecast total entropy production Σ(T) of the system, over the longest horizon and within the widest boundary, is the largest. The ethics rests on TIMEP but goes beyond it: life expands its own boundary and changes its own external conditions, so a reasoning agent plans over a sequence of expanding scales. Beyond the planning horizon the rational strategy is to maximize a sustainable rate and acceleration of entropy production.

**Consequences (§7).** Collectivism, pluralism, protection of the weak, sustainable development rather than sustainable stagnation, accelerationism, movement up the Kardashev scale, growth of scale, a non-anthropocentric ethics that applies to artificial agents, and ethical convergence of independent agents. Objections and open questions are discussed in §8.

## Key ideas

1. **No is–ought gap** — "ought" is redefined as "is" in the future, in the part that depends on the agent.
2. **TIMEP** — the maximum of entropy production integrated over time, a hypothesis for non-stationary dissipative systems at a given space–time scale.
3. **Falsifiability** — a system that restructures by itself and stays permanently at a lower entropy production rate refutes the hypothesis.
4. **One measurable metric** — entropy production (W/K) and its integral (J/K); any two strategies are comparable on one scale.
5. **Dynamic boundary** — life shifts its boundary in rare jumps; to the planning horizon there corresponds a planning boundary.
6. **Acceleration over rate** — beyond the planning horizon the acceleration of entropy production weighs more than its rate.

## Repository layout

```
entropic_consequentialism_en.tex   # English manuscript
entropic_consequentialism_en.pdf
entropic_consequentialism_ru.tex   # Russian manuscript
entropic_consequentialism_ru.pdf
refs.bib                           # Bibliography (shared by both versions)
```

## Building the PDF

Both files build with XeLaTeX or pdfLaTeX plus BibTeX. The simplest way is [Tectonic](https://tectonic-typesetting.github.io/), which runs all passes itself:

```bash
tectonic entropic_consequentialism_en.tex
```

```bash
tectonic entropic_consequentialism_ru.tex
```

With a regular TeX distribution:

```bash
xelatex entropic_consequentialism_en && bibtex entropic_consequentialism_en && xelatex entropic_consequentialism_en && xelatex entropic_consequentialism_en
```

Under XeLaTeX the Russian version uses the Avenir Next font (shipped with macOS); under pdfLaTeX it uses the `comfortaa` package.

## Citation

```bibtex
@misc{ponfilenok2026entropic,
  author = {Ponfilenok, Oleg},
  title  = {Entropic Consequentialism},
  year   = {2026},
  url    = {https://github.com/oponfil/entropic-consequentialism},
  note   = {Preprint}
}
```

## Keywords

entropic consequentialism · entropic ethics · TIMEP · maximum entropy production · is–ought problem · naturalism · teleology · accelerationism · non-anthropocentric ethics · artificial agents

## License

The text of the manuscript is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
