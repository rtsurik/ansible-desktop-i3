## ansible-desktop-i3

### Description

This role installs i3 components, Firefox and some other apps.

It should works on Debian 8/9 and Ubuntu 16.04 and above.


### Role variables:

```
desktop_user
```

The role expects that the path to the home directory is /home/{{desktop_user}}.


### Usage example:
```  become: true
  become_user: root
  become_method: sudo
  hosts: all
  vars:
    desktop_user: rustam 
  roles:
    - ansible-desktop-i3
```

