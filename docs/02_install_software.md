---
title: "Install software"
---

<div style="height: 2em;"></div>


## Installing R

::: {.panel-tabset}

### Windows

1. Go to [CRAN](https://cran.r-project.org/){target="_blank"}
2. Click **Download R for Windows**
3. Click **install R for the first time**
4. Click **Download R-X.X.X for Windows** (where X.X.X is the version number)
5. Open the downloaded installer
6. Follow the installation wizard

### macOS

1. Go to [CRAN](https://cran.r-project.org/){target="_blank"}
2. Click **Download R for macOS**
    - If you have an Apple silicon (M-series) chip, click the link ending in `arm64.pkg`
    - If you have an Intel chip, click the link ending in `x86_64.pkg`
3. Open the downloaded installer
4. Follow the installation wizard

Actually, I use another method involving `rig`, introduced [later](03_update_software.md#updating-r). However, the setup for that is more complex. If this is your first time, it is enough to follow the instructions above.

:::


## Installing RStudio

::: {.panel-tabset}

### Windows

1. Go to [Posit.io](https://docs.posit.co/ide/user/#rstudio-ide-oss-downloads){target="_blank"}
2. Click the download link beside Windows (ending in `.exe`)
3. Open the downloaded installer
4. Follow the installation wizard

### macOS

1. Go to [Posit.io](https://docs.posit.co/ide/user/#rstudio-ide-oss-downloads){target="_blank"}
2. Click the download link beside macOS 13+ (ending in `.dmg`)
3. Open the downloaded installer
4. Follow the installation wizard

:::


## Creating a GitHub account

1. Go to [GitHub.com](https://github.com/){target="_blank"}
2. Click **Sign up** on the top right corner
3. If you are a student or teacher, it is best to use your institutional email address as your primary email because you can get perks (to be discussed later in [GitHub Education](04_github_education.md))
4. Set up two-factor authentication
5. If the option comes up, select "Stay signed in" - or at least, don't log out, as we will repeatedly visit GitHub.com


## Installing Git

::: {.panel-tabset}

### Windows

1. Go to the [Git installation page](https://git-scm.com/install/){target="_blank"}
2. Click the **Windows** tab
    - If you have an Intel or AMD processor, click **Click here to download** at the top
    - If you have an ARM device (e.g., Qualcomm Snapdragon), click **Git for Windows/ARM64 Setup**
3. Open the downloaded installer
4. Follow the installation wizard
5. Confirm that Git has been installed successfully
    - Open the Terminal app (**Search > Terminal**)
    - Run `git --version` and hit Enter
    - Something like `git version 2.55.0` should appear
6. Configure your Git user information
    - In the Terminal, run `git config --global user.name "Your Name"`, replacing the `Your Name` placeholder with your full name
    - Run `git config --global user.email "your_email@example.com"`, replacing the `your_email@example.com` placeholder with an email address associated with your GitHub account
    - Confirm what you entered is correct by running `git config --global user.name` and `git config --global user.email`
    - Note that this step simply specifies the name and email that will be stamped on your Git contributions (called *commits*, which we will define commits during the bootcamp). It is unrelated to GitHub authentication. You will authenticate with GitHub the first time you do something that involves Git communicating with GitHub (e.g., when you push a commit - more on this during the bootcamp), at which point you will be prompted to authenticate using a method such as by setting up a [Personal Access Token](https://github.com/settings/tokens){target="_blank"}.

### macOS

1. Go to the [Git installation page](https://git-scm.com/install/){target="_blank"}
2. Click the **macOS** tab
    - As it notes, you will need a package installer first. Package managers are like the App Store but for software that programmers and developers will use (command-line tools and apps). Homebrew is very popular and is the easiest for new users.
3. Install Homebrew
    - Click **homebrew**
    - Copy the command underneath **Install Homebrew** by clicking the clipboard symbol. Note that although it displays a `$` before `/bin/bash ...`, you do not need to copy the leading `$`, which simply indicates that it is a Terminal command.
    - Open your Terminal app (**Spotlight > Terminal**)
    - Paste the command and hit Enter
    - To give administrative access, enter your Mac's password (hidden) and hit Enter
    - Hit Enter again to begin installation
    - After installation, it will tell you `Next steps` of which the important step is to run the commands it suggests in your Terminal to add Homebrew to your `PATH`. Copy those lines of code and paste it into the terminal and hit Enter.
4. Install Git using Homebrew
    - Returning to the Git installation page, you will see that the instructions tell you to enter `brew install git`. Copy this command; again, you do not need to copy the leading `$`.
    - Paste the command into your Terminal and hit Enter
    - When it prompts you to confirm installation `[y/n]`, type `y`
5. Confirm that Git has been installed successfully
    - In the Terminal, run `git --version` and hit Enter
    - Something like `git version 2.55.0` should appear
6. Configure your Git user information
    - In the Terminal, run `git config --global user.name "Your Name"`, replacing the `Your Name` placeholder with your full name
    - Run `git config --global user.email "your_email@example.com"`, replacing the `your_email@example.com` placeholder with an email address associated with your GitHub account
    - Confirm what you entered is correct by running `git config --global user.name` and `git config --global user.email`
    - Note that this step simply specifies the name and email that will be stamped on your Git contributions (called *commits*, which we will define commits during the bootcamp). It is unrelated to GitHub authentication. You will authenticate with GitHub the first time you do something that involves Git communicating with GitHub (e.g., when you push a commit - more on this during the bootcamp), at which point you will be prompted to authenticate using a method such as by setting up a [Personal Access Token](https://github.com/settings/tokens){target="_blank"}.

:::


## Installing Visual Studio (VS) Code

::: {.panel-tabset}

### Windows

1. Go to the [Visual Studio Code installation page](https://code.visualstudio.com/download?_exp_download=fb315fc982){target="_blank"}
2. Click the blue **Windows** button; it should automatically detect what processor you are using (Intel/AMD (x64) or ARM64)
3. Open the downloaded installer
4. Follow the installation wizard
5. If it asks you to **Continue with GitHub** to sign in, I recommend doing so. This step is optional and signs into your VS Code account via GitHub for syncing your settings, extensions, themes, etc. across devices. This is not the same as GitHub authentication.


### macOS

1. Go to the [Visual Studio Code installation page](https://code.visualstudio.com/download?_exp_download=fb315fc982){target="_blank"}
2. Click blue **Mac** button; it should automatically detect what chip you are using (Apple silicon (M-series) or Intel)
3. Open the downloaded installer
4. Follow the installation wizard
5. If it asks you to **Continue with GitHub** to sign in, I recommend doing so. This step is optional and signs into your VS Code account via GitHub for syncing your settings, extensions, themes, etc. across devices. This is not the same as GitHub authentication.

:::
