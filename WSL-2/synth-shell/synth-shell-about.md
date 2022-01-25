# `synth-shell-about.md`

## 🍅 Sauce

Video:  
[🍅 Fancy Bash Prompt! Customize Linux Terminal with SYNTH-SHELL](https://www.youtube.com/watch?v=jS-QZKjAd-U)

Repo:  
[🍅 synth-shell](https://github.com/andresgongora/synth-shell)

Dependency:
[🍅 Hack](https://github.com/source-foundry/Hack)

---

<details>
<summary>
Install `synth-shell-prompt` on Windows + WSL 2
</summary>

## Installing `synth-shell-prompt` on Windows + WSL 2

Backup your `.bashrc`. For example, you could run

```
cd ~
cp .bashrc .bashrc.backup
```

Next, install the `hack-ttf` font on windows by following the instructions [here](https://github.com/source-foundry/Hack#windows). Configure each of your Windows terminals to use the `hack` font, e.g. Windows Terminal as well as the VS code terminal fonts. For the former, you can edit the settings for the Ubuntu profile to use the `hack` font. For the latter, you can add

```
"terminal.integrated.fontFamily": "hack"
```

to the global `settings.json`. Finally, run

```
cd ~
git clone --recursive https://github.com/andresgongora/synth-shell.git
```

to download the configuration script to your home directory. Run

```
chmod +x synth-shell/setup.sh
```

to make `setup.sh` executable. Finally run

```
cd synth-shell
./setup.sh
```

to execute the script. Follow the instructions and make sure you choose to install `synth-shell-prompt`.

</details>

<details>
<summary>
Configure `synth-shell-prompt` on Windows + WSL 2
</summary>

The config file is

```
~/.config/synth-shell/synth-shell-prompt.config
```

The color names like `blue`, `white`, `dark-grey`, `light-purple`, etc. are probably ANSI colors that are overwritten by the color-scheme for the Ubuntu profile on Windows Terminal, VS Code extensions, and the `terminal` options in `settings.json`.

To manually create a color-scheme for Windows Terminal, see [this link](https://github.com/MicrosoftDocs/terminal/blob/main/TerminalDocs/install.md#configuration) as well as [this one](https://github.com/MicrosoftDocs/terminal/blob/main/TerminalDocs/customize-settings/color-schemes.md). To look at examples, refer to [here](https://terminalsplash.com/).

To manually create a color-scheme for the VS Code terminal, refer to the `settings.json` parameters in [the docs](https://code.visualstudio.com/api/references/theme-color#integrated-terminal-colors). Otherwise, examples can be found [here](https://glitchbone.github.io/vscode-base16-term/#/).

</details>
