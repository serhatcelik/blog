---
search:
  boost: 0.5
---

# VirtualBox DnD

```bash
for cmd in $(ps aux | grep "VBoxClient --draganddrop" | grep -v grep | tr -s " " | cut -d " " -f 2); do kill -2 $cmd; done
```
