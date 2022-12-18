cf-scp
======

Script to copy data via scp to CloudFoundry instances. This follows the [official guide of CloudFoundry](https://docs.cloudfoundry.org/devguide/deploy-apps/ssh-apps.html#other-ssh-access).

### Usage

```
# cf-scp $APP_NAME:$SOURCE $TARGET
cf-scp my_fancy_app:/tmp/data.json /tmp/data.json
```

You can also copy the other way round:

```
# cf-scp $SOURCE $APP_NAME:$TARGET
cf-scp /tmp/data.json my_fancy_app:/tmp/data.json
```


Required tools:

* Node.js
* scp
* sshpass
* CloudFoundry CLI
