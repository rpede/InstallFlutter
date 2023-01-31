# Flutter Setup on MacOS

**Warning I don't have a Mac to test the instructions on**

Note: execute the commands from the terminal. Type **terminal** in Spotlight.

Get [Homebrew/brew](https://brew.sh/) if you don't have it already.

Brew ia a CLI package manager for for Mac OS.

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Install git if you don't have it already.
```sh
brew install git
```

If you are on the new Apple Silicon Mac you need to install the translation layer for x86 code.

```sh
sudo softwareupdate --install-rosetta --agree-to-license
```

Now get flutter directly from github
```sh
cd ~
git clone https://github.com/flutter/flutter.git -b stable
```

Now you need to figure out what shell you are using.
```sh
echo $SHELL
```

Edit `$HOME/.bashrc` or `$HOME/.zshrc` depending on the output.

Add following line at the end of the file
```sh
export PATH="$PATH:$HOME/flutter/bin"
```

Save and reboot.

Run following command to check flutter dependencies:
```sh
flutter doctor
```

Install **Chrome** if missing.

## Visual Studio Code

Install Visual Studio Code
```sh
brew install --cask visual-studio-code
```

Open and the highlighted (yellow) extensions.

![](./screenshots/vscode.png)
