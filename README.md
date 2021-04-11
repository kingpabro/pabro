pabro
=====
##### Cracking an MD5 hash with '''hashcat'''
> hashcat -m 0 -a 0 erdew454332df3 /usr/share/wordlists/rockyou.txt

-m 0 This is the mode of attack for MD5 hashes
For MD4 hashes, use 900 as the mode.

-a 0 This is the attack mode Straight

##### Cracking MD5 hashes with John the ripper
> john --wordlist=/usr/share/wordlists/rockyou.txt --format=raw-MD5 hashes_text_file.txt

```
 just change the format to crack sha1 hashes
 ```


##### How to crack a Private key's passphrase password with John the Ripper and rockyou wordlists.
```locate ssh2john ```

``` cp /usr/share/john/ssh2john.py <path to file> python ssh2john.py idrsa.id_rsa > id.txt ```

``` john --wordlist=/usr/share/wordlists/rockyou.txt id.txt ```
