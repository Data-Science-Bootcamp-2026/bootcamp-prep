---
title: "Update software (optional)"
---

<div style="height: 2em;"></div>


## Updating R

When a new version of R is released, you can update it - though you do not have to. For instance, if you are in the middle of a project, it is simpler to keep going on the older version of R than update then verify all the code still works the same.

Patches (e.g., 4.6.0 → 4.6.1) and minor releases (e.g., 4.5 → 4.6) usually don't change much so you will rarely feel the difference. By contrast, major releases (e.g., 4 → 5) might produce breaking changes.

::: {.callout-note}
## **Note**
Updating R will not update the packages (the package maintainers may have updates for new R releases). You will still need to do that manually - we will cover this during the bootcamp.
:::

::: {.panel-tabset}

### Windows

1. Follow the same steps for [installing R](02_install_software.md#installing-r) for Windows
2. This is a bit unusual in that it downloads the new R version as a new app - it does not overwrite the previous R version
    - Yes, this takes up disk space, but this is intentional so it doesn't break your past/ongoing projects that depend on the previous version
    - Don't uninstall previous versions if you have ongoing projects
3. In RStudio, switch between R versions by:
    - **Tools > Global Options...**
    - Click the **General** tab
    - At the top, beside **R version:**, click **Change...**
    - Select the latest R version and click **OK**
    - Close RStudio and open it again
    - Upon reopening, the console (bottom left quadrant of RStudio) should state the new R version
4. If you wish to remove the previous R version, then uninstall it. Again, this is optional. I like to keep several previous R versions so that I can still run past projects.
    - (Option 1) **Settings > Apps > Installed apps**
        - Scroll down to **R for Windows X.X.X** (placeholder for the previous R version)
        - Click **...**
        - Click **Uninstall**
    - **Control Panel > Programs > Uninstall a program**
        - Scroll down to **R for Windows X.X.X** (placeholder for the previous R version)
        - Left-click and click **Uninstall** on the toolbar, or right-click and click **Uninstall** on the pop-up

### macOS

1. Follow the same steps for [installing R](02_install_software.md#installing-r) for macOS
2. Unlike Windows, installing from CRAN will overwrite your previous R installation. This is not always a good thing; follow the steps below if you do not want this behaviour.
    - Note that because the default behaviour is to overwrite your previous R installation, RStudio will not give you an option to switch between R versions as it would on Windows
3. To install and switch between multiple R versions, use `rig`, a tool developed by Posit (the same people who made RStudio)
    - Technically, `rig` also works for Windows, but the Windows RStudio already has a convenient version switcher so it is not necessary
    - Go to [their GitHub page](https://github.com/r-lib/rig){target="_blank"}
    - They offer both an installer and Homebrew installation for macOS. The installer includes both a menu bar app (GUI) as well as the command-line tool (to be run on Terminal (CLI)). The Homebrew installation only gives you the command-line tool, which may be enough if you are comfortable with CLI.
    - If you follow the link to download the installer:
        - If you have an Apple silicon (M-series) chip, click the link ending in `macOS-arm64.pkg`
        - If you have an Intel chip, click the link ending in `macOS-x86_64.pkg`
        - Open the downloaded installer
        - Follow the installation wizard
    - If you follow the instructions to install via Homebrew:
        - Open the Terminal app
        - Copy and paste the commands in the instructions
    - The menu bar app (GUI) is self-explanatory. Instead, let us introduce some common `rig` commands on the Terminal (CLI):
        - `rig --version` confirms successful installation; something like `RIG -- The R Installation Manager 0.8.1` should appear
        - `rig add release` installs the latest stable version of R; similarly, `rig add X.X.X` installs a particular R version
        - `rig list` lists installed R versions, with the default (active) version denoted with a leading `*`
        - `rig default NAME` (where `NAME` is a placeholder; use the name listed in the `rig list` output) sets that particular R version as default
        - `rig rm NAME` (where `NAME` is a placeholder; use the name listed in the `rig list` output) uninstalls that particular R version
        - `brew upgrade --cask rig` updates rig

:::


## Updating RStudio

RStudio will prompt you if an update is available.


## Updating Git

::: {.panel-tabset}

### Windows

1. Open the Terminal app
2. Run `git --version` to confirm you are behind the latest release
3. Follow the same steps for [installing Git](02_install_software.md#installing-git) for Windows

### macOS

1. Open the Terminal app
2. Run `git --version` to confirm you are behind the latest release
3. Run `brew update` to update Homebrew
4. Run `brew upgrade git` to update git
5. When it prompts you to confirm installation `[y/n]`, type `y`

:::


## Updating VS Code

VS Code will prompt you if an update is available.
