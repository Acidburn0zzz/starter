user_image
=====
sets the User's local account image

note: this is broken under 10.10.2 8\(
-----
**requires:**
\(none\)

```yaml
playbook use:
  - role: user_image
    image_name: (path to image, relative to pwd)
```