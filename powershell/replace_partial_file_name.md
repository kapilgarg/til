# Rename a file by replacing a part of existing name
```powershell
ls *.pdf | Rename-Item -NewName {$_.name -replace "December","12"}
```
