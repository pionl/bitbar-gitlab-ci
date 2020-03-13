# ![BitBar](https://github.com/matryer/bitbar/raw/master/Docs/bitbar-32.png) BitBar plugin for GitLab CI

Shows currently running pipelines from your GitLab in your bar.

![BitBar Example showing BitCoins plugin](./gitlab_ci.png)

**Interested in more advanced GitLab bar integration? Let me know (martin@kluska.cz). This implementation is just quick solution.**

## Install

Copy the plugin to your BitBar plugins directory. Edit the file and add your gitlab instances to `INSTANCES`.

```
INSTANCES = [
    {
        # Your private key for accessing gitlab: User -> Settings -> Access tokens -> add personal access token with api scope
        'privateToken': 'token',
        # Gitlab URL
        'url': 'https://gitlab.example.com',
        # Define your server and projects (name: id)
        # To get id go to project -> Settings -> General -> General project settings
        'projects': {
            "React": 3,
        },
    },
]
```

> Ensure that the gitlab url is working (urlopen does not follow redirects) #1

--- 

If you have long builds, change the refresh rate (by changing file name).

