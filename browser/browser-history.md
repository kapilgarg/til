# Firefox | Windows10
1. Browser history as a sqlite database is located at C:\Users\<user-name>\AppData\Roaming\Mozilla\Firefox\Profiles\<profile-name>
2. Type about:profiles in browser
   1. List all the profiles for current user along with their location
3. selected profile folder has a places.sqlite file which contains the browsing history
4. open this file using a sqlite client
   1. places_moz is the table which contains data