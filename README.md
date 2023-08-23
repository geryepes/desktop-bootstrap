# Prepare the new debian desktop

### Install ansible package:
> ```
> sudo apt-get install ansible
> ```
### Run the ansible playbook
> ```
> ansible-playbook bootstrap_my_pc.yaml
> ```
### Sync local files and configs:
> In the origin:
> ```
> sudo rsync -avr --files-from=include-files.txt ~/ /<bkp_disk>/
> ```
> In the destination:
> ```
> sudo rsync -av /<bkp_disk>/ ~/ 
> ```