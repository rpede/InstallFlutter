# Flutter setup on Linux

Open a terminal.

```sh
cd ~
git clone https://github.com/flutter/flutter.git -b stable
```

You need to figure out what shell you are using.

```sh
echo $SHELL
```

Edit `$HOME/.bashrc` or `$HOME/.zshrc` depending on the output.

Add following line at the end of the file:

```sh
export PATH="$PATH:$HOME/flutter/bin"
```

Logout and back in again.

Install **Chrome** you don't have it already.

If you rather use Chromium instead Chrome, then you also need to add the following to your shells configuration file (`.bashrc` or `.zshrc`).

```sh
export CHROME_EXECUTABLE="`which chromium`"
```

Run:

```sh
flutter doctor
```

You should have a checkmark on the following items

```
[✓] Flutter
[✓] Chrome - develop for the web
```

Next you will install Android toolchain and Android Studio.

[Continue](./android_studio.md)