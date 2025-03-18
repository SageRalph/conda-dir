# conda-dir

A Bash script to automatically activate a Conda environment when opening a terminal in a specific directory.

## Installation

```
curl -sS https://raw.githubusercontent.com/SageRalph/conda-dir/main/conda-dir | sudo install /dev/stdin /usr/local/bin/conda-dir
```

## Usage

Set auto-activation for the current directory:

```
conda-dir myenv
```

Remove auto-activation for the current directory:

```
conda-dir --remove
```

List existing rules:

```
conda-dir --list
```

## How It Works

- Adds a rule in `~/.bash_profile` to activate the specified Conda environment when opening a terminal in the current directory.
- Running again in the same directory with a new env name will change it.
- Removing a rule cleans it up completely.
- Works in Linux, macOS, and WSL (any Bash-based terminal).

MIT License.
