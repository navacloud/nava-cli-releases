# nava

`nava` is the command-line tool for Nava inference: deploy models, get their
endpoint URLs, manage API keys and your team, and chart traffic and latency,
all from the terminal.

## Install

macOS and Linux (Intel and ARM):

```sh
curl -fsSL https://github.com/navacloud/nava-cli-releases/releases/latest/download/install.sh | sh
```

It installs `nava` into `~/.local/bin`, checks the download against
`checksums.txt`, and offers to set up Tab completion. Run it again to update.

Options go after `sh -s --`:

```sh
curl -fsSL …/install.sh | sh -s -- v0.3.0               # a specific version
curl -fsSL …/install.sh | sh -s -- --dir /usr/local/bin # somewhere else (may need sudo)
curl -fsSL …/install.sh | sh -s -- --no-completion      # skip Tab completion
```

Or download `nava_<version>_<os>_<arch>.tar.gz` from
[Releases](https://github.com/navacloud/nava-cli-releases/releases), check it
against `checksums.txt`, and put `nava` on your `PATH`.

## Get started

```sh
nava login                      # log in in your browser and pick your organization
nava deployment create          # deploy a model, step by step
nava keys create                # make a key to call it with
nava deployment metrics <name>  # traffic, latency and tokens as charts
```

`nava --help` lists every command, and `nava <command> --help` shows examples.
Add `-o json` to any command for scripts.

## Support

Windows isn't supported yet. For help, contact your Nava account team.
