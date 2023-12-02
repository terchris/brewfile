# brewfile
my brewfiles

Store the brewfile for the mac. In thiis folder, run the following command to update the brewfile:
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

Thwn run the following command to install git:
```bash
brew install git
```

Then run the following command set up git:
```bash
git config --global user.name "Your Name"
git config --global user.email "
```
