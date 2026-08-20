# Model Sets

The public submissions inbox for curated model sets to be added to the
[models.machinefabric.com](https://models.machinefabric.com/manifest)
registry.

If you want MachineFabric to ship a new curated model set by default,
or you want existing curated recommendations reviewed, corrected, or
retired, propose it here. We curate every submission by hand. Once we
review a proposal and publish it to the live registry, it moves from
`submitted.txt` to `accepted.txt`.

## Submitting a model set

[**Submit a Model Set**](https://github.com/machinefabric/modelsets/issues/new?template=add-model-set.yml)

Anyone can propose a model set. A model set is a user-facing bundle of
concrete model recommendations mapped onto MachineFabric's model
slots, with a clear audience and hardware target.

### Requirements

- Every referenced model must be publicly accessible and actually exist.
- Every proposed model must be fit for the slot it fills.
- The proposal must explain the target user, hardware envelope, and
  why the chosen models belong together as a set.
- If a model depends on a capability or media def that is not already
  in the standard registry, propose that separately via
  [capfab](https://github.com/machinefabric/capfab/issues/new/choose).
- All submitted material must comply with our [code of conduct](#code-of-conduct).

## Feedback on curated recommendations

For everything that is not a brand-new model set submission, open
[Model Suggestions Feedback](https://github.com/machinefabric/modelsets/issues/new?template=feedback.yml).
Use it for:

- changing a recommendation inside an existing set
- flagging a stale, unsafe, or misleading recommendation
- suggesting that a curated set be removed or replaced
- asking questions or reporting bugs in the published curated sets

## How this repository works

```
modelsets/
├── submitted.txt    Proposal records awaiting maintainer review
├── accepted.txt     Proposal records that have been accepted and published
└── README.md
```

The flow:

1. You open either an
   [Add Model Set](https://github.com/machinefabric/modelsets/issues/new?template=add-model-set.yml) issue or a
   [Model Suggestions Feedback](https://github.com/machinefabric/modelsets/issues/new?template=feedback.yml) issue.
2. A maintainer records the proposal in `submitted.txt`. The issue
   stays open while we review it.
3. Once the change lands in the
   [canonical models registry](https://models.machinefabric.com/manifest),
   the record moves to `accepted.txt` and we close the issue with a link
   to the published result.
4. If we decide not to accept a proposal, we close the issue with a
   reason. The closed issue is the record. There is no separate rejected
   list.

There is no automation. Every step happens by hand. PRs that change
`submitted.txt` or `accepted.txt` should be opened only by maintainers
in response to a corresponding issue.

## Other channels

- [Model Suggestions Feedback](https://github.com/machinefabric/modelsets/issues/new?template=feedback.yml)

## Code of conduct

Be useful. Be specific. Don't submit misleading, malicious, or
deliberately low-quality recommendations. We will reject model
suggestions that are unsafe, fabricated, or clearly unfit for the slot
they claim to fill.

## Part of MachineFabric

Model Sets is part of the [MachineFabric](https://machinefabric.com)
project. The canonical curated model registry it feeds lives at
[models.machinefabric.com](https://models.machinefabric.com/manifest).
