# setup-auto action

_A GitHub action to set up [Auto](https://intuit.github.io/auto) release tool_

## Features

- Cross-platform: works on Linux, Windows, macOS
- Installs [pre-packaged binary](https://intuit.github.io/auto/docs/configuration/non-npm): 
  + works for non-npm projects
  + all official plugins are available
- Configures Git author to the `@github-actions[bot]`

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
