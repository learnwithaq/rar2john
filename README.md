# rar2john

Cracking Password Protected RAR file using rar2john.<br>
Step-by-Step guide<br>
<br>
Archive <i><b>filename.txt</b></i> in <i><b>filename.rar</b></i> -p12345 is password<br>
<pre> rar a -p12345 <filename.rar> > <filename.txt> </pre><br>
<br>
Capture hash of the password and save it in hash.txt<br>
<pre rar2john <filename>.rar > hash.txt </pre><br>
<br>
Cracking the hash using JohnTheRipper or Johnny<br>
<pre>john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt </pre><br>
<br>
