# Ansible Role Terragrunt

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

Ansible role for installating terragrunt executable

# Requirements


Only test with ansible 2.5 min version

# Role Variables

Available variables are listed below, along with default values (see [defaults/main.yml](https://github.com/nholuongut/ansible-role-terragrunt/blob/master/defaults/main.yml)):

### Terragrunt version 

```yaml
# By default, module will download last version
# To specify a version, use this below param
terragrunt_install_version: vX.X.X
```
### Download information

```yaml
# Directory where executable will be downloaded before installation
terragrunt_download_location: /tmp/
# Url to terragrunt binarie
terragrunt_url: "https://github.com/nholuongut/terragrunt/releases/download/{{ terragrunt_install_version }}/terragrunt_linux_amd64"
# Downloaded file name 
terragrunt_downloaded_file_name: terragrunt_linux_amd64
```

### Installation information

```yaml
# Path where to install terraform
terragrunt_execution_path: /usr/local/bin
# Execution file name for terraform
terragrunt_execution_file_name: terragrunt
```

Dependencies
------------

No dependencie

Example Playbook
----------------

```yaml
- hosts: all
  roles:
    - role: nholuongut.ansible_role_terragrunt
```
Inside *`vars/main.yml`*:
- Copy content of [defaults/main.yml](https://github.com/nholuongut/ansible-role-terragrunt/blob/master/defaults/main.yml) in your playbook's vars file if needed.
- Customize it as you like (filling role's variables)


# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟