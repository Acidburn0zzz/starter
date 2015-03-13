mackup
=====
uses [homebrew](https://github.com/homebrew/homebrew) to install [mackup](https://github.com/lra/mackup).  will also [cask](https://caskroom.io) install your cloud sync app of choice as well configure ~/.mackup.cfg accordingly.
-----
**requires:**
\- homebrew + cask

```yaml
playbook use:
  - role: mackup
    mackup_action: [backup|restore|uninstall] (default restore)
    sync_engine: [dropbox|google_drive|copy|box|file_system] (defaults to Dropbox)
    directory_name: Mackup (default)
    sync_path: (only needed when engine = file_system)
    app_sync_list:  (blank)
    app_ignore_list: (blank)
```

<!--
dropbox = dropbox
google_drive = google-drive
copy = copy
box = box-sync
-->
