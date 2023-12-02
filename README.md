# brewfile
my brewfiles


The one i use to set up a fresh installed mac is named Brewfile_initial

To install it run the following command:
```bash
brew bundle --file="Brewfile_initial"
```

It then installs all you ned to get started.

On the target you need to install brew first. 
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

##-----------------------------------------


## notes on creating a brewfile

Store the brewfile for the mac. In this folder, run the following command to update the brewfile:
```bash
brew bundle dump --describe --force --file="Brewfile_$(hostname)"
```

On the target machine, run the following command to install the brewfile:
```bash
brew bundle --file="Brewfile_$(hostname)"
```


## empty target machine
If the target machine is a brand new install of macOS you need to set up brew and git first. 

Run the following command to install brew:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Then install vs code to edit the brew file 
```bash
brew install --cask visual-studio-code
```

If there is no git.
Thwn run the following command to install git:
```bash
brew install git
```

Then run the following command set up git:
```bash
git config --global user.name "Your Name"
git config --global user.email "
```
