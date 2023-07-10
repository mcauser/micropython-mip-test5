# MicroPython MIP test 5

One in a series of example repos to test various mpremote mip installation patterns.

#### Install bleeding edge version v1.0.2 from main branch

```
$ mpremote mip install github:mcauser/micropython-mip-test5

Install github:mcauser/micropython-mip-test5
Installing github:mcauser/micropython-mip-test5/package.json to /lib
Installing: /lib//test5.py
Done
```

GitHub       | Device
:------------|:-------------
/test5.py    | /lib/test5.py

```
$ mpremote repl

>>> import test5
test5 main branch v1.0.2
```

#### Meanwhile, developer releases new version. Upgrade from v1.0.2 to v1.1.0 (latest)

```
$ mpremote mip install github:mcauser/micropython-mip-test5

Install github:mcauser/micropython-mip-test5
Installing github:mcauser/micropython-mip-test5/package.json to /lib
Installing: /lib//test5.py
Done
```

GitHub       | Device
:------------|:-------------
/test5.py    | /lib/test5.py

```
$ mpremote repl

>>> import test5
test5 main branch v1.1.0
```

#### Downgrade from v1.1.0 to v1.0.0 release

```
$ mpremote mip install github:mcauser/micropython-mip-test5@v1.0.0

Install github:mcauser/micropython-mip-test5
Installing github:mcauser/micropython-mip-test5/package.json to /lib
Installing: /lib//test5.py
Done
```

```
$ mpremote repl

>>> import test5
test5 main branch v1.0.0
```

#### Install the unreleased dev branch version v0.0.1

```
$ mpremote mip install github:mcauser/micropython-mip-test5@dev

Install github:mcauser/micropython-mip-test5
Installing github:mcauser/micropython-mip-test5/package.json to /lib
Installing: /lib//test5.py
Done
```

```
$ mpremote repl

>>> import test5
test5 dev branch v0.0.1
```
