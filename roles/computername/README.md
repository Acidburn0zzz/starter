computername
=====
set Computer's name, equivalent of using System Preferences - Sharing
-----
**requires:**<br />
\- ansible\-playbook \-K for sudo<br />

playbook use:
```yaml
  - role: computername
    computername: <foo>
```

possibly more useful:
```yaml
  vars_prompt:
    - name: "prompted_name"
      prompt: "Name of Machine?"
      private: no
  roles:
  - role: computername
    computername: "{{ prompted_name }}"
```

