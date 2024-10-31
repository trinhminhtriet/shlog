# shlog

```text
      _      _
 ___ | |__  | |  ___    __ _
/ __|| '_ \ | | / _ \  / _` |
\__ \| | | || || (_) || (_| |
|___/|_| |_||_| \___/  \__, |
                       |___/

```

A lightweight shell logging tool for tracking and managing command history with easy integration and analysis.

## ✨ Features

TBD

## 🚀 Installation

To install **shlog**, simply clone the repository and follow the instructions below:

```bash
git clone git@github.com:trinhminhtriet/shlog.git
cd shlog

cargo build --release
cp ./target/release/shlog /usr/local/bin/
```

Running the below command will globally install the `shlog` binary.

```bash
cargo install shlog
```

Optionally, you can add `~/.cargo/bin` to your PATH if it's not already there

```bash
echo 'export PATH="$HOME/.cargo/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## 💡 Usage

```bash
shlog [FLAGS] [OPTIONS]
```

```text
shlog --help

shlog 0.1.0
Triet Trinh <contact@trinhminhtriet.com>
A CLI tool for inspecting shell history

USAGE:
    shlog [FLAGS] [OPTIONS]

FLAGS:
        --flavor-bash      Manually select Bash history, overriding auto-detect
    -e, --display-exact    Show the most common exact commands
    -z, --display-fuzzy    Show fuzzy matched output. This is the default option.
    -h, --help             Prints help information
    -t, --display-heat     Show the most common command components
    -V, --version          Prints version information
        --flavor-zsh       Manually select ZSH history, overriding auto-detect

OPTIONS:
    -n <count>        How many items to show [default: 10]
    -f <file>         File to parse. Defaults to history file of selected or detected shell flavor
```

### Flags

- `--flavor-bash`: Manually select Bash history, overriding auto-detect.
- `-e`, `--display-exact`: Show the most common exact commands.
- `-z`, `--display-fuzzy`: Show fuzzy matched output (default option).
- `-h`, `--help`: Prints help information.
- `-t`, `--display-heat`: Show the most common command components.
- `-V`, `--version`: Prints version information.
- `--flavor-zsh`: Manually select ZSH history, overriding auto-detect.

### Options

- `-n <count>`: Specify how many items to show (default: 10).
- `-f <file>`: Specify the file to parse. Defaults to the history file of the selected or detected shell flavor.

With Shlog, gain valuable insights into your command history and enhance your command-line productivity. Integrate it into your workflow today!

## 🗑️ Uninstallation

Running the below command will globally uninstall the `shlog` binary.

```bash
cargo uninstall shlog
```

Remove the project repo

```bash
rm -rf /path/to/git/clone/shlog
```

## 🤝 How to contribute

We welcome contributions!

- Fork this repository;
- Create a branch with your feature: `git checkout -b my-feature`;
- Commit your changes: `git commit -m "feat: my new feature"`;
- Push to your branch: `git push origin my-feature`.

Once your pull request has been merged, you can delete your branch.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
