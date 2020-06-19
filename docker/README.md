# BlockScout Docker Integration

This integration is not production ready, and should be used for local BlockScout deployment only.

For usage instructions and ENV variables, see the [docker integration documentation](https://docs.blockscout.com/for-developers/information-and-settings/docker-integration-local-use-only).


# Windows issue

C:\Program Files\Docker\Docker\resources\bin\docker.exe: Error response from daemon: OCI runtime create failed: container_linux.go:349: starting container process caused "exec: "C:/Program Files/Git/usr/bin/sh": stat C:/Program Files/Git/usr/bin/sh: no such file or directory": unknown.
make: *** [Makefile:265: start] Error 127

On receiving this error you can change the Makefile and make the following adjustments:
From:  /bin/sh
To:    //bin/sh
