# First time configuration

The first time you use the Azure CLI it can be good to setup a few defaults.

## Azure CLI defaults

```bash
az configure --defaults location=westeurope group=test
```
It is also a good idea to set the default output format to table when you are beginning to work with Azure CLI. If not all of the outputs will be in JSON format which is hard to read on the screen.

```bash
az configure

Do you wish to change your settings? (y/N): y

What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses.
 [2] jsonc - Colored JSON formatted output that most closely matches API responses.
 [3] table - Human-readable output format.
 [4] tsv - Tab- and Newline-delimited. Great for GREP, AWK, etc.
 [5] yaml - YAML formatted output. An alternative to JSON. Great for configuration files.
 [6] none - No output, except for errors and warnings.
Please enter a choice [Default choice(3)]: 3
```

then use the defaults for the rest until you return to the prompt.

## Configure Git for your user 

```bash
git config --global user.email "<youremail>@mail.com"
git config --global user.name "Your Name"
```
# SSH keys

