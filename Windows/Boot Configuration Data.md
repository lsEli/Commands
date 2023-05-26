# Boot Configuration Data

## List EFI boot entries

```powershell
bcdedit /enum firmware
```

## Remove EFI boot entry

```powershell
bcdedit /delete {boot_entry_identifier}
```
