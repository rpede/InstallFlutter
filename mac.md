# Flutter Setup on MacOS

**Warning I don't have a Mac to test the instructions on**

Open "Terminal"

If you are on the new Apple Silicon Mac you need to install the translation layer for x86 code.

```sh
sudo softwareupdate --install-rosetta --agree-to-license
```

Now get flutter directly from github

```sh
cd ~
git clone https://github.com/flutter/flutter.git -b stable
```

You need to figure out what shell you are using.

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

Don't worry about the other issues for now.

[Continue](./android.md)