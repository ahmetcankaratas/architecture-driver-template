# Architecture Driver Template

A template for capturing **architecture drivers** — the business goals, key functional requirements, quality attributes and constraints that shape a software architecture.

| File                                                                     | Format                                                           |
| ------------------------------------------------------------------------ | ---------------------------------------------------------------- |
| [`architecture-driver-template.md`](architecture-driver-template.md)     | Markdown — copy one file per driver into your repository         |
| [`architecture-driver-template.xlsx`](architecture-driver-template.xlsx) | Excel — one sheet per driver; Status and Priority are drop-downs |

## Structure

```
Categorization    Driver Name · Driver ID · Status · Priority
Responsibilities  Supporter · Sponsor · Author · Inspector
Description       Environment · Stimulus · Response   |   Quantification
```

Fill **Environment → Stimulus → Response** in that order, then quantify each. The response is a black-box view: it says what the system does, not how. A response that cannot be measured cannot be verified.
