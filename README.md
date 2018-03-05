# freenas-plex
Plex installer on freenas

## Plex in freenas jail
Uses ansible to configure plex in a jail to make updating jails easier. Configures daemontools to monitor and restart plex service. 

Configures and installs comskip and comchap for DVR features.

## Prerequisites
```pkg install python ansible```

## Usage
1. Copy plex.yml to your jail
2. ```ansible-playbook -i "localhost," -c local -e "ansible_python_interpreter=/usr/local/bin/python2.7" plex.yml```
