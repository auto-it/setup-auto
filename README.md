# setup-auto action

_A GitHub action to set up [Auto](https://intuit.github.io/auto) release tool_

## Usage

Here's an example usage:

```yaml
jobs:
  release:
    runs-on: # ...
    steps:
      - uses: actions/checkout@v2
      - uses: laughedelic/setup-auto@v1
      - run: auto shipit
```

See [`action.yml`](./action.yml) for available inputs.
