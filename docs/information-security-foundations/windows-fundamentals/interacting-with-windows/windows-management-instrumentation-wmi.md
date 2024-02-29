---
icon: material/help
search:
  boost: 0.5
---

# Windows Management Instrumentation (WMI)

## Questions

```text
Use WMI to find the serial number of the system.
```

??? tip "Steps"

    ```powershell
    Get-WmiObject -Class win32_OperatingSystem | Select-Object -Property SerialNumber
    ```
