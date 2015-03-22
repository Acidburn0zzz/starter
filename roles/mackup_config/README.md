mackup-config
=====
configures ~/.mackup.cfg accordingly to user settings
-----
**requires:**
\- none

```yaml
playbook use:
  - role: mackup_config
    sync_engine: [dropbox|google_drive|copy|box|file_system] # (defaults to dropbox)
    directory_name: Mackup # (default)
    optional:
    sync_path: # (only needed when engine = file_system)
    app_sync_list: # (blank)
    app_ignore_list: # (blank)
```

