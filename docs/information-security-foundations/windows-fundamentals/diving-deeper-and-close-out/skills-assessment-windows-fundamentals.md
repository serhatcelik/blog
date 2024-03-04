---
icon: material/help
---

# Skills Assessment - Windows Fundamentals

## Questions

```text
What is the name of the service associated with Windows Update?
```

??? tip "Steps"

    ```powershell
    Get-Service | ? { $_.DisplayName -match "Update" }
    ```

```text
List the SID associated with the user account Jim you created.
```

??? tip "Steps"

    Yeni bir yerel kullanıcı oluştur:

    ```powershell
    New-LocalUser -Name "Jim" -NoPassword
    ```

    Kullanıcı SID bilgisini görüntüle:

    ```powershell
    wmic useraccount get name,sid | Select-String "Jim"
    ```

```text
List the SID associated with the HR security group you created.
```

??? tip "Steps"

    PowerShell üzerinde `#!powershell compmgmt` komutunu girerek Computer Management arayüzünü aç.

    Burada `Local Users and Groups` --> `Groups` yolunu takip et.

    ++right-button++ --> `New Group...` seçeneğini seç ve `HR` isminde bir grup oluştur.

    Son olarak aşağıdaki komut ile SID bilgisini öğren:

    ```powershell
    wmic group get name,sid | Select-String "HR"
    ```
