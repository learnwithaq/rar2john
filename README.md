# rar2john

Cracking Password Protected RAR file using rar2john.<br>
Step-by-Step guide<br>
<br>
Archive <filename>.txt in <filename>.rar -p12345 is password
rar a -p12345 <filename>.rar <filename>.txt<br>
<br>
Capture hash of the password and save it in hash.txt
rar2john <filename>.rar > hash.txt<br>
<br>
Cracking the hash using JohnTheRipper or Johnny<br>
john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt<br>
<br>
