# collect
Bash shell script to collect log files (i.e. text strings being written to any file), etc. from disparate Linux hosts.
The collect.sh script and its (two) included/sourced adhoc-src.\*load.txt (aka header) files should
 be copied into the /usr/local/bin directory.
A user-specific configuration file must be created in the directory /usr/local/collect/.
This configuration file must use the following naming convention:
/usr/local/collect/collect.[username].cfg
Execute as follows:
collect.sh [username]

Note that trusted hosts must be set up, using appropriate keys; this means being able to ssh onto
 remote hosts without needing to enter a password.

At least these enhancements are currently suggested/planned:
1. Allow specifying non-standard (i.e. root) username to execute as on remote hosts;
2. Allow use of sudo on remote hosts, in order to execute tcpdump.
