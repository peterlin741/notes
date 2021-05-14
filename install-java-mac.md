## How to manage different java versions on Mac

- Followed this guide (commands here not up to date)
  - https://gist.github.com/tomysmile/a9a7aee85ff73454bd57e198ad90e614
- Update home brew
  - `brew update`
  - `brew upgrade`
- Install jenv with brew to manage java environments
  - Add the below to `~/.bash_profile` to initialize jenv

```
# Init jenv
if which jenv > /dev/null; then eval "$(jenv init -)"; fi
```

  - To set the version, run `jenv local {java_version}` (for that directory) or `jenv global {java_version}`
  - Use `jenv versions` to view available versions. You can view the Java paths in `~/.jenv/versions`
  - The steps above handle setting the `JAVA_HOME` variable

- Use cask to download java versions (not handled by jenv)
  - `brew install --cask java`
  - `brew install --cask adoptopenjdk11` (also adoptopenjdk8, adoptopenjdk13)


## IntelliJ

- How to set the Java version within an IntelliJ Gradle Project
  - `Preferences > Build, Execution, Deployment > Build Tools > Gradle`
  - `Project Structure > Project Settings > Project`