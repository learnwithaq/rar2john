# rar2john

Cracking Password Protected RAR file using rar2john.<br>
Step-by-Step guide<br>
<br>
Archive <i><b>filename.txt</b></i> in <i><b>filename.rar</b></i> -p12345 is password<br><br>
rar a -p12345 <i>filename.rar</i> <i><filename.txt</i><br>
<br>
Capture hash of the password and save it in hash.txt
rar2john <filename>.rar > hash.txt<br>
<br>
Cracking the hash using JohnTheRipper or Johnny<br>
john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt<br>
<br>
