# Dotfiles
Ref: https://www.gnu.org/software/stow/manual/stow.html

## Mandatory
There is only one mandatory file for this dotfile to work, which contains all the sensitive information:
```
export USER_EMAIL="jerome.michel@symphony.com"
export USER_GITHUB="jeromeM-symphony"
export USER_GIT_NAME="JeromeM"

export AWS_ACCESS_KEY_ID="xxxxx"
export AWS_SECRET_ACCESS_KEY="xxxxx"

export ARTIFACTORY_PASSWORD="xxxxx"
```

## Configuration
By default the folder is configured with `STOW_DIR` but on the first hand, no sh config is injected. So we need to add it to the command line for the first install

## How to
### Init
```
STOW_DIR="~/dotfiles"
git clone git@github.com:jeromeM-symphony/Dotfiles.git ${STOW_DIR}
```

# To use any module
```
stow <module>
```

# To uninstall any module
```
stow -D <module>
```

# To reinstall in case of issue or new files
```
stow -R <module>
```
