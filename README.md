`My Powershell Notes`

## 𝐏𝐨𝐰𝐞𝐫𝐬𝐡𝐞𝐥𝐥 𝐍𝐨𝐭𝐞𝐬

- Powershell works with unix commands too i.e. linux commands also works in powershell.

Unix | cmd | Powershell
--- | --- | ---
cd home | cd c:\ | set-location c:\
ls | dir | get-childitem
clear | cls | clear-host
mkdir dirname | mkdir dirname | md dirname
man | help | help

---

- Powershell equivalent of `tail` command:
```
get-content filenamehere -tail 10
```

- Powershell equivalent of `grep` command
```
Get-Content .\doc.txt | Select-String -Pattern (Get-Content .\regex.txt)
```

- Powershell equivalent of `grep -r` command
```
dir -recurse | Select-String -pattern [SEARCH_PATTERN]
```
---

- Powershell equivalent of `wc -l` command
```
measure
```

- Reference: 
```
https://learn.microsoft.com/en-us/shows/getstartedpowershell3/
```
