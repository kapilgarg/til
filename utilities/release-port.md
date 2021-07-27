# Release a port which is held up by a dead process

## windows
1. Open command prompt and type `netstat -ano | findstr <port number>`
2. From the result, pick up the last column which gives the process id
3. kill the process `taskkill /F /PID <process id>`