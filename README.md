# env_setup_new_mac

## Install [Homebrew](https://brew.sh/)
  - ```/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"```

## Install [Rails Version Manager (rvm)](https://rvm.io/)
  - ```\curl -sSL https://get.rvm.io```

## Install Postgres via brew and start the service
  - ```brew install postgresql```
  - ```brew services start postgresql```

## If you run into openssl problems
  - ```brew reinstall openssl@1.1```

## Install Node Version Manager (NVM)
  - ```brew install nvm```

## Install Latest Node
  - ```nvm install --lts```

## ZSH Case Insensitive Auto-complete
  - edit `~/.zshrc ` and add the following lines:
    ```
    ## case-insensitive (uppercase from lowercase) completion
    zstyle ':completion:*' matcher-list 'm:{a-z}={A-Z}'
    ## case-insensitive (all) completion
    #zstyle ':completion:*' matcher-list 'm:{a-zA-Z}={A-Za-z}'
    ## case-insensitive,partial-word and then substring completion
    #zstyle ':completion:*' matcher-list 'm:{a-z}={A-Z}' 'r:|[._-]=* r:|=*' 'l:|=* r:|=*'
    ```
  - reload your `.zshrc` settings
    ```
    source ~/.zshrc
    ```
    
