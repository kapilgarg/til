# You can convert a folder into a new powershell drive with New-PSDrive

```
New-PSDrive foo filesystem 'C:\Program Files'
New-PSDrive bar filesystem 'foo:\Microsoft'
cd foo:
```

## To persist between sessions
1. Add them to your profile script ($profile).
2. type **$profile** on powershell prompt to get the file location. If the file is not present, create a file at this location and add the commands to that.
3. restart the powershell window.

https://stackoverflow.com/a/16598373/45280
