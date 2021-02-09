cf-scp
======

Script to copy data via scp to CloudFoundry instances. This follows the [official guide of CloudFoundry](https://docs.cloudfoundry.org/devguide/deploy-apps/ssh-apps.html#other-ssh-access).

### Usage

```cf-scp $APP_NAME $SOURCE $TARGET```

Example:

```cf-scp my_fancy_app /tmp/data.json /tmp/data.json```

Required tools:

* cf-cli
* jq
* pbcopy (for putting the one time access code to the clipboard)
* scp
