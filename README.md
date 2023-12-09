Argon EON Ansible Role
======================

An Ansible role to install Argon EON integration services to a Raspberry Pi.

Requirements
------------

None

Role Variables
--------------

- `argoneon_enable_rtc_service`: boolean, default: `yes`  
Whether to enable or disable Argon EON service for RTC

- `argoneon_enable_fan_lcd_service`: boolean, default: `yes`  
Whether to enable or disable Argon EON service for LCD and fan

Dependencies
------------

None

Example Playbook
----------------

To enable both services (default):
```yaml
- hosts: all
  roles:
    - argon-eon
```

To disable one service:
```yaml
- hosts: all
  roles:
    - role: argon-eon
      vars:
        argoneon_enable_rtc_service: no
        argoneon_enable_fan_lcd_service: yes
```

License
-------

MIT
