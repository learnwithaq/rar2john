# rar2john

Cracking Password Protected RAR file using rar2john.<br>
Step-by-Step guide<br>

rar a -p12345 <filename>.rar <filename>.txt #Archive <filename>.txt in <filename>.rar -p12345 is password
<br>
rar2john <filename>.rar > hash.txt # capture hash of the password and save it in hash.txt
<br>
john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt # Cracking the hash using JohnTheRipper or Johnny
<br>
