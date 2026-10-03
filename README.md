# Architecture Driver & Design Decision Templates

Two templates that connect _what a system must achieve_ to _how its architecture answers it_.

| File                                                                     | Format                                                    |
| ------------------------------------------------------------------------ | --------------------------------------------------------- |
| [`architecture-driver-template.md`](architecture-driver-template.md)     | Markdown — one file per **architecture driver**           |
| [`architecture-driver-template.xlsx`](architecture-driver-template.xlsx) | Excel — same template; Status and Priority are drop-downs |
| [`design-decision-template.md`](design-decision-template.md)             | Markdown — one file per **design decision**               |
| [`design-decision-template.xlsx`](design-decision-template.xlsx)         | Excel — same template                                     |

## Architecture driver

```
Categorization    Driver Name · Driver ID · Status · Priority
Responsibilities  Supporter · Sponsor · Author · Inspector
Description       Environment · Stimulus · Response   |   Quantification
```

Fill **Environment → Stimulus → Response** in that order, then quantify each. The response is a black-box view: it says what the system does, not how. A response that cannot be measured cannot be verified.

Prefix driver IDs by type: `BD` business goal, `AD` key functional requirement / quality attribute, `CO` constraint.

## Design decision

```
Decision Name · Design Decision ID · Addresses Driver · Explanation
Pros & Opportunities   |   Cons & Risks
Assumptions & Quantifications   |   Trade-Offs
Manifestation Links
```

A decision names the driver(s) it addresses and the trade-off it accepts. A driver without a decision, or a decision without a driver, is a traceability gap.
