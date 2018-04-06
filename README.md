# ![BitBar](https://github.com/matryer/bitbar/raw/master/Docs/bitbar-32.png) BitBar plugin for GitLab CI

Shows currently running pipelines from your GitLab in your bar.

![BitBar Example showing BitCoins plugin](./gitlab_ci.png)

**Interested in more advanced GitLab bar integration? Let me know (martin@kluska.cz). This implementation is just quick solution.**

## Install

Copy the plugin to your BitBar plugins directory. Edit the file and add your GitLab data.

> PRIVATE_TOKEN = 'token'

Your private key for accessing gitlab: User -> Settings -> Access tokens -> add personal access token with api scope

> URL = 'https://gitlab.example.com'

Gitlab URL

> PROJECTS ={"React": 3}

Define your projects you want to check (name: id).

To get id go to project -> Settings -> General -> General project settings.

--- 

If you have long builds, change the refresh rate (by changing file name).

