Ansible role for setup resilio sync to Linux server
Tested on Ubuntu 16.04

For use Web interface to access controle panel, nothing needs to be changed!

To configure the synchronization of the dictionaries through the configuration file config.json, you must use the varibales
but the WebUI is desable

Example:

resilio_sync_shared_folders:
  - secret: YouSuperSecretResilioKey
    dir: /dir/for/synchronization
    use_tracker: 'true' - if needed
    search_lan: 'true' - if needed
    use_sync_trash: 'true' - if needed
    selective_sync: 'true' - if needed
    overwrite_changes: 'false' - if not needed
    known_hosts: 111.222.333.444:0000 - if needed
