TOML
====

Original repository: https://github.com/uiri/toml

See also https://github.com/mojombo/toml

Python module which parses and emits TOML.

Released under the MIT license.

Passes https://github.com/BurntSushi/toml-test

See http://j.xqz.ca/toml-status for up to date test results.

Current Version of the Specification
------------------------------------

https://github.com/mojombo/toml/blob/v0.2.0/README.md

QUICK GUIDE
-----------


```
pip install toml
```


toml.loads --- takes a string to be parsed as toml and returns the corresponding dictionary

toml.dumps --- takes a dictionary and returns a string which is the contents of the corresponding toml file.


There are other functions which I use to dump and load various fragments of toml but dumps and loads will cover most usage.

Example usage:

```
import toml

with open("conf.toml") as conffile:
     config = toml.loads(conffile.read())
# do stuff with config here
. . .
```
