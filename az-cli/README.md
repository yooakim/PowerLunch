# Azure CLI

Here you will find scripts, examples and more for working with the Azure CLI.

## Requirements
All of the code and examples here require that you have access to an Azure subscription. If you don't have it you can create a trial subscription.

* Access to one or more Azure subscriptions
* Command line Git




## Install the CLI
The CLI is based on Python and can be used on Windows, macOS, Linux and in a Docker Container. 

To install the CLI in your local computer,visit [this page](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest) and chose your operating 
system for further instructions.

An even easier way to get started is to use the Azure CLI via a web browser. Simply go to the [Azure Shell](https://shell.azure.com/).


## First time configuration

The first time you use the Azure CLI it can be good to setup a few defaults.

```bash
az configure --defaults location=westeurope group=test
az configure
Welcome to the Azure CLI! This command will guide you through logging in and setting some default values.

Your settings can be found at /home/joakim/.azure/config
Your current configuration is as follows:

[cloud]
name = AzureCloud

[core]
first_run = yes
output = table
collect_telemetry = yes
cache_ttl = 10

[logging]
enable_log_file = no

[defaults]
location = westeurope
group = test

Environment variables:
AZURE_ACCESS_TOKEN_FILE = /tmp/accessTokens.json
AZURE_HTTP_USER_AGENT = cloud-shell/1.0

Do you wish to change your settings? (y/N): y

What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses.
 [2] jsonc - Colored JSON formatted output that most closely matches API responses.
 [3] table - Human-readable output format.
 [4] tsv - Tab- and Newline-delimited. Great for GREP, AWK, etc.
 [5] yaml - YAML formatted output. An alternative to JSON. Great for configuration files.
 [6] none - No output, except for errors and warnings.
Please enter a choice [Default choice(3)]: 3

Would you like to enable logging to file? (y/N): n

Microsoft would like to collect anonymous Azure CLI usage data to improve our CLI.  Participation is voluntary and when you choose to participate, your device automatically sends information to Microsoft about how you use Azure CLI.  To update your choice, run "az configure" again.
Select y to enable data collection. (Y/n):

CLI object cache time-to-live (TTL) in minutes [Default: 10]:

You're all set! Here are some commands to try:
 $ az login
 $ az vm create --help
 $ az feedback
```
