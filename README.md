Bash Json Parser
================

JSON Parser in pure bash

Exposes a `json-parse` function that will read a JSON string given on stdin
and sets a global variable JSONREPLY with the parsed data.

Usage
-----

```bash
json-parse <<< '{"foo":"bar"}' || exit 1
echo "${JSONREPLY[foo]}"
# => "bar"
```

License
-------

MIT License
