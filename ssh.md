- Add the following to your `~/.ssh/config` file to prevent prompting for your ssh key
```
Host *
  IgnoreUnknown AddKeysToAgent,UseKeychain
  AddKeysToAgent yes
  UseKeychain yes
  IdentityFile ~/.shh/id_rsa
 ```
