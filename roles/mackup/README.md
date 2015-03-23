mackup
=====
uses [homebrew](https://github.com/homebrew/homebrew) to install [mackup](https://github.com/lra/mackup).  will also [cask](https://caskroom.io) install your cloud sync app of choice as well configure ~/.mackup.cfg accordingly.
-----
**requires:**
\- homebrew + cask

```yaml
playbook use:
  - role: mackup
    sync_engine: [dropbox|google_drive|copy|box|file_system] # (defaults to dropbox)
    sync_dir: Mackup # (default)
```

