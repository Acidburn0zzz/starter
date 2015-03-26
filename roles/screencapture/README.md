screencapture
==========

this allows the customization of apple's builtin screencapture's image format and location.
----------

**requires:**<br />

```yaml
playbook use:
  - role: screencapture
    ## optional:
    screencap_img_type: [png|pdf|jpg|tif|psd] # png default
    screencap_location: /path/to/foo # ~/Desktop default, will be created it needed
```