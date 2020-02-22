# Set up macOS for Stardew Valley modding

This guide assumes that you already know a lot of things. If you need help with something, please feel free to open an issue and I'll be happy to answer questions and add information to the guide! Also, it assumes you're using Bash as your shell. If you don't know what that means, don't worry about it; if you're using a different shell, I expect you're enough of a power-user to account for the differences.

## 0. Install Homebrew

> **Homebrew** is a package manager for macOS.

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
echo "export HOMEBREW_CASK_OPTS=\"--appdir=/Applications\"" >> ~/.bash_profile
source ~/.bash_profile
```

## 1. Install Mono

> **Mono** is an open source implementation of Microsoft's .NET Framework based on the Ecma standards for C# and the <abbr title="Common Language Runtime">CLR</abbr>.

```bash
brew install mono mono-libgdiplus
```

## 2. Install SMAPI

> **SMAPI** is the **S**tardew **M**odding **<abbr title="Application Programming Interface">API</abbr>**.

1. Go to the [**For mod creators**][0] section at the bottom of [SMAPI's website][1], and click on **SMAPI x.x.x for developers** to download the SMAPI installer.
2. Run:

    ```bash
    unzip SMAPI-3.2.0-installer-for-developers.zip
    ./SMAPI-3.2.0-installer-for-developers.zip
    ```

[0]: https://smapi.io/#modcreators
[1]: https://smapi.io/
