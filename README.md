# Pinguino IDE 13

This repository contains the Pinguino IDE 13 codebase. Pinguino is an integrated development environment for working with supported microcontroller boards and the associated Pinguino toolchain and libraries.

This README covers obtaining the IDE and libraries, launching the application, and configuring the compiler paths.

## Project components

The Pinguino development environment uses two repositories:

- [Pinguino IDE](https://github.com/PinguinoIDE/pinguino-ide) — the IDE source.
- [Pinguino libraries](https://github.com/PinguinoIDE/pinguino-libraries) — the associated device libraries.

The compiler toolchains are separate dependencies and must also be available on your system.

## Get the source

Create a workspace and clone both repositories:

```bash
mkdir -p ~/Pinguino/v13
cd ~/Pinguino/v13

git clone https://github.com/PinguinoIDE/pinguino-ide.git pinguino-ide
git clone https://github.com/PinguinoIDE/pinguino-libraries.git pinguino-libraries
```

If you are using this repository as your IDE source, clone this repository in place of the upstream IDE URL while keeping the libraries repository alongside it.

Your workspace should contain:

```text
Pinguino/
└── v13/
    ├── pinguino-ide/
    └── pinguino-libraries/
```

## Launch the IDE

Run the launcher for your platform from the IDE directory.

**Python launcher:**

```bash
python pinguino-ide.py
```

**Windows:**

```bat
pinguino.bat
```

**Linux:**

```bash
./pinguino.sh
```

The Python launcher requires the dependencies expected by the Pinguino IDE source. If the application does not start, check its console output and verify that the required Python packages and compiler tools are installed.

## Configure compiler and library paths

The IDE configuration files are located at:

- Linux: `pinguino/qtgui/config/pinguino.linux.conf`
- Windows: `pinguino/qtgui/config/pinguino.windows.conf`

Edit the configuration file for your operating system and set the paths to the toolchains and libraries installed on your machine.

The relevant settings are:

```ini
[Paths]
sdcc_bin = "full_path_to_pinguino-compilers"/p8/bin
gcc_bin = "full_path_to_pinguino-compilers"/p32/bin
xc8_bin = "full_path_to_xc8"/bin
pinguino_8_libs = "full_path_to_pinguino-ide"/p8
pinguino_32_libs = "full_path_to_pinguino-ide"/p32
install_path = "full_path_to_pinguino-ide"

user_path = ~/Pinguino/v13
user_libs = ${user_path}/pinguinolibs
```

Replace the example paths with the actual locations on your system. The compiler paths must point to the directories containing the corresponding executables.

## Updating the source

From each cloned repository, pull the latest changes:

```bash
cd ~/Pinguino/v13/pinguino-ide
git pull

cd ~/Pinguino/v13/pinguino-libraries
git pull
```

Keep local changes backed up before updating if you have modified either repository.

## Support and bug reports

For issues with the upstream Pinguino IDE project, see the [Pinguino IDE issue tracker](https://github.com/PinguinoIDE/pinguino-ide/issues).

This repository's code and its upstream dependencies may have their own licensing and contribution terms. Check the relevant license files before redistributing modified versions.
