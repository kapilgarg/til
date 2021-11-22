# Windows 10
## Chrome: Disable private browsing and guest mode 
[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome]
"IncognitoModeAvailability"=dword:00000001
"BrowserGuestModeEnabled"=dword:00000000

## Edge: Disable private browsing and guest mode 
[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Edge]
"InPrivateModeAvailability"=dword:00000001
"BrowserGuestModeEnabled"=dword:00000001
  
