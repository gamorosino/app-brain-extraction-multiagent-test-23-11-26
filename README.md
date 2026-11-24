# app-brain-extraction-multiagent-test-23-11-26

Skull-strip a T1w volume using FSL's BET.

## Inputs

- `t1w` (neuro/anat/t1w)

## Outputs

- `t1_brain` (neuro/anat/t1w) -- Brain-extracted T1w volume

## Usage

Brainlife.io: run via `faber-app-run`/`faber-app-pipeline` (once registered
with `faber-app-create`), or the web UI.

Locally (outside brainlife): copy `config.json.example` to `config.json`,
fill in real file paths, then run `./main` from this directory. `main` pulls
its own container (`singularity exec docker://...`) -- no local install of
the underlying tool needed, only Singularity itself.

Entrypoint: `run_bet.sh`

## Authors

- Gabriele Amorosino <g.amorosino@gmail.com>

#### MIT Copyright (c) 2026 Gabriele Amorosino
