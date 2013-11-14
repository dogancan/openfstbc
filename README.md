Bash completion file for OpenFst 1.3.4

Copyright Paul Dixon 2011 (paul@edobashira.com)

Bash 3 (Mac OS X) support by Dogan Can (dogancan@usc.edu)

Tested on Ubuntu 10.04 using bash 4.5, Mac OS 10.9 using bash 3.2.

---

To use simply source the completion file.

    source openfstbc          # for Bash 4
    source openfstbc-bash3    # for Bash 3 (Mac OS X)

These bash completions will add tab completion to OpenFst flags. This file adds three types of completions based on the flag’s value type.

* Flags which accept a path or a numeric value will complete with a trailing `=` character and then default to the standard path completion.

* Binary flags will complete without a trailing `=` character.

* Flags which accept an enumerable string value will complete with a trailing `=` and then suggest suitable values. For example `--arc_type=` completions will suggest `log` and `standard`.