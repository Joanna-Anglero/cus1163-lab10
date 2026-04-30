Analysis Questions:
1. A world-writable directory is more dangerous than a world-writable file because it gives the attackers control of what is in the directory. With this, an attacker can upload and replace files with corrupt ones that will harm the system if opened. 
2. -Perm -002 means that all of the bits in the file must be set, while -perm /111 means any of the bits can be set. We use different options because each of their goals produces a different output.
3. If I ran this scanner on a production web server and found 50 world-writable files, the immediate actions I would take would be to remove the writable files that may cause harm to the system, find where the problem has occurred, and make sure that there is better security for it.
4. Find ... | while read does not work for counting because the loop runs in a subshell due to the pipe and < < (find ...) processes substitution, allowing for it to work properly. 
5. I would schedule this script by adding the code to a path and telling the code to scan the file during the specific time, and even have an alert for it if an error occurs. 
