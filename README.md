# rar2john

Cracking Password Protected RAR file using rar2john.<br><br>
Step-by-Step guide<br>
<br>
Archive <i><b>filename.txt</b></i> in <i><b>filename.rar</b></i> -p12345 is password<br>
<pre> rar a -p12345 <i>filename.rar</i> > <i>filename.txt</i> </pre><br>

Capture hash of the password and save it in hash.txt<br>
<pre> rar2john <i>filename.rar</i> > hash.txt </pre><br>

Cracking the hash using JohnTheRipper or Johnny<br>
<pre>john --wordlist=/usr/share/wordlists/rockyou.txt hash.txt </pre><br>
