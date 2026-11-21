# Auto clipper bot

Open-access clipping website: no admin panel and no required account at initial launch.
Processing is performed on a user's own Google Colab runtime, connected through a temporary pairing token.

## Architecture (initial scaffold)
- `web/`: frontend starter placeholder
- `colab/`: Colab worker notebook source (Python)
- `docs/source-inventory.md`: inspection notes from `clipping_agent.zip`

Security design note: open access is not equivalent to private storage. A future persistent project/account feature will need authentication or explicit per-project access tokens.
