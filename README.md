# devSetup
a guide to my dev setup

# aliases
- ldb = local Postgres while running navy

```alias ldb="docker exec -it $(docker ps --filter "name=postgres" --format "{{.Names}}") psql -U postgres"```

- rn = rename
- clp = postgres with psgci (needs fixing with password)

``` 
rename() {
  printf '\e]2;%s\a' "$*";
}
alias rn=rename
alias clp='rn local-pg && set PGPASSWORD=caughtwithmyplantsdown && pgcli -h localhost -p $(navy port postgres 5432) -U postgres'
```

- rnra = run android simulator

```alias rnra='react-native run-android'```



# VSCode install
Extensions:
 - Apollo GraphQL
 - markdownlint - David Anson
 - EditorConfig
 - gitlens - Eric Amodio
 - shell-format - foxundermoon
 - graphql-for-vscode
 - Todo Highlight
 - vscode-icons


# install git 
```sudo apt install git-all```

```git config --g user.name <NAME>```

```git config --g user.email <EMAIL>```

```git config --global pull.rebase true```

```git config --global rebase.autoStash true```


# enable ssh
 - https://support.atlassian.com/bitbucket-cloud/docs/set-up-an-ssh-key/

# install Curl
```sudo apt install curl ```

# install homebrew
https://www.osradar.com/install-homebrew-ubuntu-20-04-debian-10/

# install nvm & node
 - https://tecadmin.net/how-to-install-nvm-on-ubuntu-20-04/
 
 - ```curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash```
 
 - ```nvm alias default 12.20.1```
 
 - currently installed
 
 - run: npm login 
 

# android studio / react native setup
https://reactnative.dev/docs/environment-setup
 - download android studio
 
 - use AVD Manager make device using Android Q(10)
 
 - ```sudo apt-get install openjdk-8-jdk```
 
 - ensure ./bashrc contains paths to android/java (as per article)
 
 - ```brew install watchman```
 
 - ```npm install -g react-native-cli```
 
 
 # Successfully Launched dev version
 - Visiting-CMS-UI
 
 - CMS-UI
 
 - Website (localhost:8080) might need to change .env for navy?
 
 - Mobile App in android sim

# Install Docker, Compose & Navy
 - https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04
 - Step 1 & 2 then restart Machine
 
 - Install Docker Compose
https://linuxize.com/post/how-to-install-and-use-docker-compose-on-ubuntu-18-04/

 - Follow steps in floating garden readme: https://bitbucket.org/candide-garden-app/floating-garden/src/master/

 - Install GCloud SDK https://cloud.google.com/sdk/docs/quickstart#deb

# Install Magic Wormhole file transfer
 - ```sudo apt install magic-wormhole```
 
# Install Insomnia
 - In Software / snap
