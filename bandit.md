<h1> bandit 0 </h1>
<p> Login via ssh:
<br><b>sh -l bandit0 bandit.labs.overthewire.org -p 2220</b>
<br> with password: <i>bandit0</i>
</p>
<p><b>bandit0@bandit:~$ ls</b>
<pre>readme</pre>
<b>bandit0@bandit:~$ cat readme</b>
<pre>boJ9jbbUNNfktd78OOpsqOltutMc3MY1</pre></p>
<p> Password to next level is: boJ9jbbUNNfktd78OOpsqOltutMc3MY1</p>

<h1> bandit 1 </h1>
<p><b>bandit1@bandit:~$ cat ./- </b>
<pre>CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9</pre></p>
<p> Password to next level is: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9</p>
<h1> bandit 2 </h1>
<p><b>bandit2@bandit:~$ cat spaces\ in\ this\ filename</b>
<pre>UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK</pre></p>
<p> Password to next level is: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK</p>
<h1> bandit 3 </h1>
<p><b>bandit3@bandit:~$ cd inhere/</b>
<br><b>bandit3@bandit:~/inhere$ ls -la</b>
<pre>total 12
drwxr-xr-x 2 root    root    4096 Nov 14  2014 .
drwxr-xr-x 3 root    root    4096 Nov 14  2014 ..
-rw-r----- 1 bandit4 bandit3   33 Nov 14  2014 .hidden</pre>
<b>bandit3@bandit:~/inhere$ cat .hidden</b>
<pre>pIwrPrtPN36QITSp3EQaw936yaFoFgAB</pre></p>
<p> Password to next level is: pIwrPrtPN36QITSp3EQaw936yaFoFgAB</p>

<h1> bandit 4 </h1>
<p><b>bandit4@bandit:~$ cd inhere/</b>
<br><b>bandit4@bandit:~/inhere$ ls -la</b>
<pre>total 48
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file00
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file01
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file02
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file03
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file04
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file05
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file06
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file07
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file08
-rw-r----- 1 bandit5 bandit4   33 Nov 14  2014 -file09
drwxr-xr-x 2 root    root    4096 Oct 19  2016 .
drwxr-xr-x 3 root    root    4096 Nov 14  2014 ..</pre>
<b>bandit4@bandit:~/inhere$</b>
<br><b>bandit4@bandit:~/inhere$ cat ./-file07</b>
<pre>koReBOKuIDDepwhWk7jZC0RTdopnAYKh</pre></p>
<p> Password to next level is: koReBOKuIDDepwhWk7jZC0RTdopnAYKh</p>

<h1> bandit 5 </h1>
<p><b>bandit5@bandit:~$ ls</b>
<pre>inhere</pre>
<b>bandit5@bandit:~$ cd inhere/</b>
<br><b>bandit5@bandit:~/inhere$ ls -la</b>
<pre>total 88
drwxr-x--- 22 root bandit5 4096 Nov 14  2014 .
drwxr-xr-x  3 root root    4096 Nov 14  2014 ..
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere00
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere01
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere02
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere03
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere04
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere05
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere06
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere07
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere08
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere09
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere10
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere11
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere12
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere13
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere14
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere15
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere16
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere17
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere18
drwxr-x---  2 root bandit5 4096 Nov 14  2014 maybehere19</pre>
<b>bandit5@bandit:~/inhere$ find . -type f -readable ! -executable -size 1033c</b>
<pre>./maybehere07/.file2</pre>
<b>bandit5@bandit:~/inhere$ cat ./maybehere07/.file2</b>
<pre>DXjZPULLxYr17uwoI01bNLQbtFemEgo7</pre></p>
<p> Password to next level is: DXjZPULLxYr17uwoI01bNLQbtFemEgo7</p>

<h1> bandit 6 </h1>
<p><b>bandit6@bandit:~$ find / -user bandit7 -group bandit6 -size 33c 2>/dev/null</b>
<pre>/var/lib/dpkg/info/bandit7.password</pre>
<b>bandit6@bandit:~$ cat /var/lib/dpkg/info/bandit7.password</b>
<pre>HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs</pre></p>
<p> Password to next level is: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs</p>

<h1> bandit 7</h1>
<p><b>bandit7@bandit:~$ ls</b>
<pre>data.txt</pre>
<b>bandit7@bandit:~$ cat data.txt | grep "millionth"</b>
<pre>millionth cvX2JJa4CFALtqS87jk27qwqGhBM9plV</pre></p>
<p> Password to next level is: cvX2JJa4CFALtqS87jk27qwqGhBM9plV</p>

<h1> bandit 8 </h1>
<p><b>bandit8@bandit:~$ ls</b>
<pre>data.txt</pre>
<b>bandit8@bandit:~$ cat data.txt | sort | uniq -u</b>
<pre>UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR</pre></p>
<p> Password to next level is: cvX2JJa4CFALtqS87jk27qwqGhBM9plV</p>

<h1> bandit 9</h1>
<p><b>bandit9@bandit:~$ ls</b>
<pre>data.txt</pre>
<b>bandit9@bandit:~$ strings data.txt | grep "="</b>
<pre>epr~F=K
7?YD=
?M=HqAH
/(Ne=
C=_"
I========== the6
z5Y=
`h(8=`
n\H=;
========== password
========== ism
N$=&
l/a=L)
f=C(
========== truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
ie)=5e</pre></p>
<p> Password to next level is: truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk</p>

<h1> bandit 10 </h1>
<p><b>bandit10@bandit:~$ ls</b>
<pre>data.txt</pre>
<b>bandit10@bandit:~$ cat data.txt</b>
<pre>VGhlIHBhc3N3b3JkIGlzIElGdWt3S0dzRlc4TU9xM0lSRnFyeEUxaHhUTkViVVBSCg==</pre>
<b>bandit10@bandit:~$ cat data.txt | base64 --decode</b>
<pre>The password is IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR</pre></p>
<p> Password to next level is: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR</p>

<h1> bandit 11</h1>
<p><b>bandit11@bandit:~$ ls</b>
<pre>data.txt</pre>
<b>bandit11@bandit:~$ cat data.txt</b>
<pre>Gur cnffjbeq vf 5Gr8L4qetPEsPk8htqjhRK8XSP6x2RHh</pre>
<b>bandit11@bandit:~$ cat data.txt | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'</b>
</pre>The password is 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu</pre></p>
<p> Password to next level is: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu</p>

<h1> bandit 12 </h1>
<p><b>bandit12@bandit:~$ ls</b>
<pre>data.txt</pre>
<b>bandit12@bandit:~$ mkdir /tmp/hgcs</b>
<br><b>bandit12@bandit:~$ cp data.txt /tmp/hgcs</b>
<br><b>bandit12@bandit:~$ cd /tmp/hgcs</b>
<br><b>bandit12@bandit:/tmp/hgcs$ ls</b>
<pre>data.txt</pre>
<b>bandit12@bandit:/tmp/hgcs$ file data.txt</b>
<pre>data.txt: ASCII text</pre>
<b>bandit12@bandit:/tmp/hgcs$ xxd -r data.txt > data_xxd_reverse</b>
<br><b>bandit12@bandit:/tmp/hgcs$ file data_xxd_reverse</b>
<pre>data_xxd_reverse: gzip compressed data, was "data2.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression</pre>
<b>bandit12@bandit:/tmp/hgcs$ zcat data_xxd_reverse > data_zcat</b>
<b>bandit12@bandit:/tmp/hgcs$ file data_zcat</b>
<pre>data_zcat: bzip2 compressed data, block size = 900k</pre>
<b>bandit12@bandit:/tmp/hgcs$ bzip2 -d data_zcat</b>
<pre>bzip2: Can't guess original name for data_zcat -- using data_zcat.out</pre>
<b>bandit12@bandit:/tmp/hgcs$ file data_zcat.out</b>
<pre>data_zcat.out: gzip compressed data, was "data4.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression</pre>
<b>bandit12@bandit:/tmp/hgcs$ zcat data_zcat.out > data_zcat_2</b>
<br><b>bandit12@bandit:/tmp/hgcs$ file data_zcat_2</b>
<pre>data_zcat_2: POSIX tar archive (GNU)</pre>
<b>bandit12@bandit:/tmp/hgcs$ tar xvf data_zcat_2</b>
<pre>data5.bin</pre>
<b>bandit12@bandit:/tmp/hgcs$ file data5.bin</b>
<pre>data5.bin: POSIX tar archive (GNU)</pre>
<b>bandit12@bandit:/tmp/hgcs$ tar xvf data5.bin</b>
<pre>data6.bin</pre>
<b>bandit12@bandit:/tmp/hgcs$ file data6.bin</b>
<pre>data6.bin: bzip2 compressed data, block size = 900k</pre>
<b>bandit12@bandit:/tmp/hgcs$ bzip2 -d data6.bin</b>
<pre>bzip2: Can't guess original name for data6.bin -- using data6.bin.out</pre>
<b>bandit12@bandit:/tmp/hgcs$ file data6.bin.out</b>
<pre>data6.bin.out: POSIX tar archive (GNU)</pre>
<b>bandit12@bandit:/tmp/hgcs$ tar xvf data6.bin.out</b>
<pre>data8.bin</pre>
<b>bandit12@bandit:/tmp/hgcs$ file data8.bin</b>
<pre>data8.bin: gzip compressed data, was "data9.bin", from Unix, last modified: Fri Nov 14 10:32:20 2014, max compression</pre>
<b>bandit12@bandit:/tmp/hgcs$ zcat data8.bin > data8_zcat</b>
<br><b>bandit12@bandit:/tmp/hgcs$ file data8_zcat</b>
<pre>data8_zcat: ASCII text</pre>
<b>bandit12@bandit:/tmp/hgcs$ cat data8_zcat</b>
<pre>The password is 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL</pre></p>
<p> Password to next level is: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL</p>

<h1> bandit 13 </h1>
<p><b>bandit13@bandit:~$ ls</b>
<pre>sshkey.private</pre>
<b>bandit13@bandit:~$ file sshkey.private</b>
<pre>sshkey.private: PEM RSA private key</pre>
<b>bandit13@bandit:~$ cat sshkey.private</b>
<pre>-----BEGIN RSA PRIVATE KEY-----
MIIEpAIBAAKCAQEAxkkOE83W2cOT7IWhFc9aPaaQmQDdgzuXCv+ppZHa++buSkN+
gg0tcr7Fw8NLGa5+Uzec2rEg0WmeevB13AIoYp0MZyETq46t+jk9puNwZwIt9XgB
ZufGtZEwWbFWw/vVLNwOXBe4UWStGRWzgPpEeSv5Tb1VjLZIBdGphTIK22Amz6Zb
ThMsiMnyJafEwJ/T8PQO3myS91vUHEuoOMAzoUID4kN0MEZ3+XahyK0HJVq68KsV
ObefXG1vvA3GAJ29kxJaqvRfgYnqZryWN7w3CHjNU4c/2Jkp+n8L0SnxaNA+WYA7
jiPyTF0is8uzMlYQ4l1Lzh/8/MpvhCQF8r22dwIDAQABAoIBAQC6dWBjhyEOzjeA
J3j/RWmap9M5zfJ/wb2bfidNpwbB8rsJ4sZIDZQ7XuIh4LfygoAQSS+bBw3RXvzE
pvJt3SmU8hIDuLsCjL1VnBY5pY7Bju8g8aR/3FyjyNAqx/TLfzlLYfOu7i9Jet67
xAh0tONG/u8FB5I3LAI2Vp6OviwvdWeC4nOxCthldpuPKNLA8rmMMVRTKQ+7T2VS
nXmwYckKUcUgzoVSpiNZaS0zUDypdpy2+tRH3MQa5kqN1YKjvF8RC47woOYCktsD
o3FFpGNFec9Taa3Msy+DfQQhHKZFKIL3bJDONtmrVvtYK40/yeU4aZ/HA2DQzwhe
ol1AfiEhAoGBAOnVjosBkm7sblK+n4IEwPxs8sOmhPnTDUy5WGrpSCrXOmsVIBUf
laL3ZGLx3xCIwtCnEucB9DvN2HZkupc/h6hTKUYLqXuyLD8njTrbRhLgbC9QrKrS
M1F2fSTxVqPtZDlDMwjNR04xHA/fKh8bXXyTMqOHNJTHHNhbh3McdURjAoGBANkU
1hqfnw7+aXncJ9bjysr1ZWbqOE5Nd8AFgfwaKuGTTVX2NsUQnCMWdOp+wFak40JH
PKWkJNdBG+ex0H9JNQsTK3X5PBMAS8AfX0GrKeuwKWA6erytVTqjOfLYcdp5+z9s
8DtVCxDuVsM+i4X8UqIGOlvGbtKEVokHPFXP1q/dAoGAcHg5YX7WEehCgCYTzpO+
xysX8ScM2qS6xuZ3MqUWAxUWkh7NGZvhe0sGy9iOdANzwKw7mUUFViaCMR/t54W1
GC83sOs3D7n5Mj8x3NdO8xFit7dT9a245TvaoYQ7KgmqpSg/ScKCw4c3eiLava+J
3btnJeSIU+8ZXq9XjPRpKwUCgYA7z6LiOQKxNeXH3qHXcnHok855maUj5fJNpPbY
iDkyZ8ySF8GlcFsky8Yw6fWCqfG3zDrohJ5l9JmEsBh7SadkwsZhvecQcS9t4vby
9/8X4jS0P8ibfcKS4nBP+dT81kkkg5Z5MohXBORA7VWx+ACohcDEkprsQ+w32xeD
qT1EvQKBgQDKm8ws2ByvSUVs9GjTilCajFqLJ0eVYzRPaY6f++Gv/UVfAPV4c+S0
kAWpXbv5tbkkzbS0eaLPTKgLzavXtQoTtKwrjpolHKIHUz6Wu+n4abfAIRFubOdN
/+aLoRQ0yBDRbdXMsZN/jvY44eM+xRLdRVyMmdPtP8belRi2E2aEzA==
-----END RSA PRIVATE KEY-----</pre>
<b>bandit13@bandit:~$ ssh bandit14@localhost -i sshkey.private -p 2220</b>
<br><b>bandit13@bandit:~$ cat /etc/bandit_pass/bandit14</b>
<pre>4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e</pre></p>
<p> Password to next level is: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e</p>

<h1> bandit 14 </h1>
<p><b>bandit14@bandit:~$ nc localhost 30000</b>
<pre>4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr</pre></p>
<p> Password to next level is: BfMYroe26WYalil77FoDi9qh59eK5xNr</p>

<h1> bandit 15 </h1>
<p><b>bandit15@bandit:~$ openssl s_client -connect localhost:30001 -ign_eof</b>
<pre>CONNECTED(00000003)
depth=0 CN = li190-250.members.linode.com
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = li190-250.members.linode.com
verify return:1
---
Certificate chain
 0 s:/CN=li190-250.members.linode.com
   i:/CN=li190-250.members.linode.com
---
Server certificate
-----BEGIN CERTIFICATE-----
MIIC3jCCAcagAwIBAgIJAI5QiWZw4YHbMA0GCSqGSIb3DQEBCwUAMCcxJTAjBgNV
BAMTHGxpMTkwLTI1MC5tZW1iZXJzLmxpbm9kZS5jb20wHhcNMTQxMTE0MTAyODA0
WhcNMjQxMTExMTAyODA0WjAnMSUwIwYDVQQDExxsaTE5MC0yNTAubWVtYmVycy5s
aW5vZGUuY29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAsKmy9o5z
WU+1EH7Z3bB5TGQA+16zXDcEJy6tZWZ8CDrRyQXiahendp45BWUc/ZuLDo0+B3Wt
ZXjofmLw/F4fmR+8X1s1fQZX2dFt920qEm7LxqzWd0c7FdHiBwwRrwhkk+3cQpOB
TTGdLWEgpdmwwNZDTUdsDLzjDczPnju6T6p6ArTECztPbmTjfY4QIRtC6capL1Z+
yPJSQVAuAMEX1wTDWTGdm0VV7oW4F5cGZutf6QAP51jdhSyZuGilIPHbnj0l6Qc7
a7+OtEsEGi31aJ8KpRf7LNZ7DXCuoB3Hf75Pd6VjDgoOIagcH0NYqa75gEjBkGzs
ktLWykT7ag7fKwIDAQABow0wCzAJBgNVHRMEAjAAMA0GCSqGSIb3DQEBCwUAA4IB
AQCaZdUNAj8WDEKWdoU3LNXUBJlTJwiWBrh550PbHSQORcCz2K0kiMei1A4ojK2N
dMHFGAqAeUEaxtz92p2BoFpZasAtdSa3u63tBckFhfUolIS1TC7Cj51y19ysTeep
fGPFpuPCVqVPsruei8Z/iqn3bFIhQQdmumeePZQdPMwZSWHNVYC5XODd7PvNDrDu
5MZJjkz4+6LbwwAvyew62meFN2QEsYbK2Brtbhze+IjE27FGWlSw4K3jlwa409MD
MTf4JU41ELaYY8G/LSNDJsBVhhkHzvXR9iCbXxNz3IL0dQDNj7h4LKhBy0q7hvqg
kDzwlmBO4WKSmCAuky44cXmd
-----END CERTIFICATE-----
subject=/CN=li190-250.members.linode.com
issuer=/CN=li190-250.members.linode.com
---
No client certificate CA names sent
---
SSL handshake has read 1714 bytes and written 637 bytes
---
New, TLSv1/SSLv3, Cipher is DHE-RSA-AES256-SHA
Server public key is 2048 bit
Secure Renegotiation IS supported
Compression: NONE
Expansion: NONE
SSL-Session:
    Protocol  : SSLv3
    Cipher    : DHE-RSA-AES256-SHA
    Session-ID: 3D3C8090F26497A5D8EC930C9D4B09A577BE6E4872070FE6FB59CB073B6F9EDA
    Session-ID-ctx:
    Master-Key: E73F17121DE4869A375F9683213BD9C6F742B74819AD2A2AD69A37931DA57499C45CFFDAAEB1AE708EE83C6082EB67A2
    Key-Arg   : None
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    Start Time: 1495332494
    Timeout   : 300 (sec)
    Verify return code: 18 (self signed certificate)
---
BfMYroe26WYalil77FoDi9qh59eK5xNr
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd
read:errno=0</pre></p>
<p> Password to next level is: cluFn7wTiGryunymYOu4RcffSxQluehd</p>

<h1> bandit 16 </h1>
<p><b>bandit16@bandit:~$ nmap -sT -A -p 31000-32000 localhost</b>
<pre>Starting Nmap 7.70 ( http://nmap.org ) at 2019-05-21 02:18 UTC
Nmap scan report for localhost (127.0.0.1)
Host is up (0.00037s latency).
Not shown: 996 closed ports
PORT      STATE SERVICE VERSION
31046/tcp open  echo
31518/tcp open  msdtc   Microsoft Distributed Transaction Coordinator (error)
31691/tcp open  echo
31790/tcp open  msdtc   Microsoft Distributed Transaction Coordinator (error)
31960/tcp open  echo
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows
Service detection performed. Please report any incorrect results at http://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 41.29 seconds</pre>
<b>bandit16@bandit:~$ openssl s_client -connect localhost:31790</b>
<pre>CONNECTED(00000003)
depth=0 CN = li190-250.members.linode.com
verify error:num=18:self signed certificate
verify return:1
depth=0 CN = li190-250.members.linode.com
verify return:1
---
Certificate chain
 0 s:/CN=li190-250.members.linode.com
   i:/CN=li190-250.members.linode.com
---
Server certificate
-----BEGIN CERTIFICATE-----
MIIC3jCCAcagAwIBAgIJAI5QiWZw4YHbMA0GCSqGSIb3DQEBCwUAMCcxJTAjBgNV
BAMTHGxpMTkwLTI1MC5tZW1iZXJzLmxpbm9kZS5jb20wHhcNMTQxMTE0MTAyODA0
WhcNMjQxMTExMTAyODA0WjAnMSUwIwYDVQQDExxsaTE5MC0yNTAubWVtYmVycy5s
aW5vZGUuY29tMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAsKmy9o5z
WU+1EH7Z3bB5TGQA+16zXDcEJy6tZWZ8CDrRyQXiahendp45BWUc/ZuLDo0+B3Wt
ZXjofmLw/F4fmR+8X1s1fQZX2dFt920qEm7LxqzWd0c7FdHiBwwRrwhkk+3cQpOB
TTGdLWEgpdmwwNZDTUdsDLzjDczPnju6T6p6ArTECztPbmTjfY4QIRtC6capL1Z+
yPJSQVAuAMEX1wTDWTGdm0VV7oW4F5cGZutf6QAP51jdhSyZuGilIPHbnj0l6Qc7
a7+OtEsEGi31aJ8KpRf7LNZ7DXCuoB3Hf75Pd6VjDgoOIagcH0NYqa75gEjBkGzs
ktLWykT7ag7fKwIDAQABow0wCzAJBgNVHRMEAjAAMA0GCSqGSIb3DQEBCwUAA4IB
AQCaZdUNAj8WDEKWdoU3LNXUBJlTJwiWBrh550PbHSQORcCz2K0kiMei1A4ojK2N
dMHFGAqAeUEaxtz92p2BoFpZasAtdSa3u63tBckFhfUolIS1TC7Cj51y19ysTeep
fGPFpuPCVqVPsruei8Z/iqn3bFIhQQdmumeePZQdPMwZSWHNVYC5XODd7PvNDrDu
5MZJjkz4+6LbwwAvyew62meFN2QEsYbK2Brtbhze+IjE27FGWlSw4K3jlwa409MD
MTf4JU41ELaYY8G/LSNDJsBVhhkHzvXR9iCbXxNz3IL0dQDNj7h4LKhBy0q7hvqg
kDzwlmBO4WKSmCAuky44cXmd
-----END CERTIFICATE-----
subject=/CN=li190-250.members.linode.com
issuer=/CN=li190-250.members.linode.com
---
No client certificate CA names sent
---
SSL handshake has read 1714 bytes and written 637 bytes
---
New, TLSv1/SSLv3, Cipher is DHE-RSA-AES256-SHA
Server public key is 2048 bit
Secure Renegotiation IS supported
Compression: NONE
Expansion: NONE
SSL-Session:
    Protocol  : SSLv3
    Cipher    : DHE-RSA-AES256-SHA
    Session-ID: 20CA4FD2722C9FC893DECEE1CA87C16F698563B7116265F39D48D3D8F6853EAF
    Session-ID-ctx:
    Master-Key: FE0F0C093E12801D5CF052F1734410396EF1D35B1C85BA0DA685ED8A990E62A96221321469CA02D4C7374A628EDEECE8
    Key-Arg   : None
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    Start Time: 1495333239
    Timeout   : 300 (sec)
    Verify return code: 18 (self signed certificate)
---
cluFn7wTiGryunymYOu4RcffSxQluehd
Correct!
-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAvmOkuifmMg6HL2YPIOjon6iWfbp7c3jx34YkYWqUH57SUdyJ
imZzeyGC0gtZPGujUSxiJSWI/oTqexh+cAMTSMlOJf7+BrJObArnxd9Y7YT2bRPQ
Ja6Lzb558YW3FZl87ORiO+rW4LCDCNd2lUvLE/GL2GWyuKN0K5iCd5TbtJzEkQTu
DSt2mcNn4rhAL+JFr56o4T6z8WWAW18BR6yGrMq7Q/kALHYW3OekePQAzL0VUYbW
JGTi65CxbCnzc/w4+mqQyvmzpWtMAzJTzAzQxNbkR2MBGySxDLrjg0LWN6sK7wNX
x0YVztz/zbIkPjfkU1jHS+9EbVNj+D1XFOJuaQIDAQABAoIBABagpxpM1aoLWfvD
KHcj10nqcoBc4oE11aFYQwik7xfW+24pRNuDE6SFthOar69jp5RlLwD1NhPx3iBl
J9nOM8OJ0VToum43UOS8YxF8WwhXriYGnc1sskbwpXOUDc9uX4+UESzH22P29ovd
d8WErY0gPxun8pbJLmxkAtWNhpMvfe0050vk9TL5wqbu9AlbssgTcCXkMQnPw9nC
YNN6DDP2lbcBrvgT9YCNL6C+ZKufD52yOQ9qOkwFTEQpjtF4uNtJom+asvlpmS8A
vLY9r60wYSvmZhNqBUrj7lyCtXMIu1kkd4w7F77k+DjHoAXyxcUp1DGL51sOmama
+TOWWgECgYEA8JtPxP0GRJ+IQkX262jM3dEIkza8ky5moIwUqYdsx0NxHgRRhORT
8c8hAuRBb2G82so8vUHk/fur85OEfc9TncnCY2crpoqsghifKLxrLgtT+qDpfZnx
SatLdt8GfQ85yA7hnWWJ2MxF3NaeSDm75Lsm+tBbAiyc9P2jGRNtMSkCgYEAypHd
HCctNi/FwjulhttFx/rHYKhLidZDFYeiE/v45bN4yFm8x7R/b0iE7KaszX+Exdvt
SghaTdcG0Knyw1bpJVyusavPzpaJMjdJ6tcFhVAbAjm7enCIvGCSx+X3l5SiWg0A
R57hJglezIiVjv3aGwHwvlZvtszK6zV6oXFAu0ECgYAbjo46T4hyP5tJi93V5HDi
Ttiek7xRVxUl+iU7rWkGAXFpMLFteQEsRr7PJ/lemmEY5eTDAFMLy9FL2m9oQWCg
R8VdwSk8r9FGLS+9aKcV5PI/WEKlwgXinB3OhYimtiG2Cg5JCqIZFHxD6MjEGOiu
L8ktHMPvodBwNsSBULpG0QKBgBAplTfC1HOnWiMGOU3KPwYWt0O6CdTkmJOmL8Ni
blh9elyZ9FsGxsgtRBXRsqXuz7wtsQAgLHxbdLq/ZJQ7YfzOKU4ZxEnabvXnvWkU
YOdjHdSOoKvDQNWu6ucyLRAWFuISeXw9a/9p7ftpxm0TSgyvmfLF2MIAEwyzRqaM
77pBAoGAMmjmIJdjp+Ez8duyn3ieo36yrttF5NSsJLAbxFpdlc1gvtGCWW+9Cq0b
dxviW8+TFVEBl1O4f7HVm6EpTscdDxU+bCXWkfjuRb7Dy9GOtt9JPsX8MBTakzh3
vBgsyi/sN3RqRBcGU40fOoZyfAMT8s1m/uYv52O6IgeuZ/ujbjY=
-----END RSA PRIVATE KEY-----
read:errno=0</pre>
connect to bandit17@localhost using this ssh private key.
<br><b>[$]-> mkdir /tmp/mykey</b>
<br><b>[$]-> nano /tmp/mykey/sshkey.pem</b>

<br>## PASTE IN THE PRIVATE KEY THEN SAVE AND EXIT

<br><b>[$]-> chmod 600 /tmp/mykey/sshkey.pem</b>
<br><b>[$]-> ssh -i /tmp/mykey/sshkey.pem bandit17@localhost</b>

<h1> bandit 17 </h1>
<p><b>bandit16@bandit:~$ ls</b>
<pre>passwords.new  passwords.old</pre>
<b>bandit16@bandit:~$ file *</b>
<pre>passwords.new: ASCII text
passwords.old: ASCII text</pre>
<b>bandit16@bandit:~$ diff passwords.new passwords.old</b>
<pre>42c42
< kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd</pre></p>
<p> Password to next level is: kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd</p>

<h1> bandit 18 </h1>
<p><b>[~]$ ssh bandit18@bandit.labs.overthewire.org -p 2220</b>
<pre>Byebye !</pre>
<p><b>[~]$ ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme</b>
<pre>This is the OverTheWire game server. More information on http://www.overthewire.org/wargames
Please note that wargame usernames are no longer level<X>, but wargamename<X>
e.g. vortex4, semtex2, ...
Note: at this moment, blacksun is not available.
bandit18@bandit.labs.overthewire.org's password:
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x</pre></p>
<p> Password to next level is: IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x</p>

<h1> bandit 19 </h1>
<p><b>bandit19@bandit:~$ ls</b>
<pre>bandit20-do</pre>
<b>bandit19@bandit:~$ file bandit20-do</b>
<pre>bandit20-do: setuid ELF 32-bit LSB  executable, Intel 80386, version 1 (SYSV), dynamically linked (uses shared libs), for GNU/Linux 2.6.24, BuildID[sha1]=08e74b8e092a91103efaab7916d75f08b887ab4d, not stripped</pre>
<b>bandit19@bandit:~$ ls -la bandit20-do</b>
<pre>-rwsr-x--- 1 bandit20 bandit19 7370 Nov 14  2014 bandit20-do</pre>
<b>bandit19@bandit:~$ ./bandit20-do</b>
<pre>Run a command as another user.
  Example: ./bandit20-do id</pre>
<b>bandit19@bandit:~$ ./bandit20-do id</b>
<pre>uid=11019(bandit19) gid=11019(bandit19) euid=11020(bandit20) groups=11020(bandit20),11019(bandit19)</pre>
<b>bandit19@bandit:~$ ./bandit20-do whoami</b>
<pre>bandit20</pre>
<b>bandit19@bandit:~$ ./bandit20-do cat /etc/bandit_pass/bandit20</b>
<pre>GbKksEFF4yrVs6il55v6gwY5aVje5f0j</pre></p>
<p> Password to next level is: GbKksEFF4yrVs6il55v6gwY5aVje5f0j</p>

<h1> bandit 20</h1>
<p><b>bandit20@bandit:~$ ls -la suconnect</b>
<pre>-rwsr-x--- 1 bandit21 bandit20 8006 Nov 14  2014 suconnect</pre>
<b>bandit20@bandit:~$ ./suconnect</b>
<pre>Usage: ./suconnect <portnumber>
This program will connect to the given port on localhost using TCP. If it receives the correct password from the other side, the next password is transmitted back.</pre>
</pre></p>
create nc chat in then get
<p> Password to next level is: gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr</p>

<h1> bandit 21 </h1>
<p><b>bandit21@bandit:~$ ls</b>
<br><b>bandit21@bandit:~$ cd /etc/cron.d/</b>
<br><b>bandit21@bandit:/etc/cron.d$ ls -l</b>
<pre>total 92
-r--r----- 1 root root  46 Nov 14  2014 behemoth4_cleanup
-rw-r--r-- 1 root root 355 May 25  2013 cron-apt
-rw-r--r-- 1 root root  61 Nov 14  2014 cronjob_bandit22
-rw-r--r-- 1 root root  62 Nov 14  2014 cronjob_bandit23
-rw-r--r-- 1 root root  61 May  3  2015 cronjob_bandit24
-rw-r--r-- 1 root root  62 May  3  2015 cronjob_bandit24_root
-r--r----- 1 root root  47 Nov 14  2014 leviathan5_cleanup
-rw------- 1 root root 233 Nov 14  2014 manpage3_resetpw_job
-rw-r--r-- 1 root root  51 Nov 14  2014 melinda-stats
-rw-r--r-- 1 root root  54 Jun 25  2016 natas-session-toucher
-rw-r--r-- 1 root root  49 Jun 25  2016 natas-stats
-r--r----- 1 root root  44 Jun 25  2016 natas25_cleanup
-r--r----- 1 root root  47 Aug  3  2015 natas25_cleanup~
-r--r----- 1 root root  47 Jun 25  2016 natas26_cleanup
-r--r----- 1 root root  43 Jun 25  2016 natas27_cleanup
-rw-r--r-- 1 root root 510 Oct 29  2014 php5
-rw-r--r-- 1 root root  63 Jul  8  2015 semtex0-32
-rw-r--r-- 1 root root  63 Jul  8  2015 semtex0-64
-rw-r--r-- 1 root root  64 Jul  8  2015 semtex0-ppc
-rw-r--r-- 1 root root  35 Nov 14  2014 semtex5
-rw-r--r-- 1 root root 396 Nov 10  2013 sysstat
-rw-r--r-- 1 root root  29 Nov 14  2014 vortex0
-rw-r--r-- 1 root root  30 Nov 14  2014 vortex20</pre>
<b>bandit21@bandit:/etc/cron.d$ cat cronjob_bandit22</b>
<pre>* * * * * bandit22 /usr/bin/cronjob_bandit22.sh &> /dev/null</pre>
<b>bandit21@bandit:/etc/cron.d$ cat /usr/bin/cronjob_bandit22.sh</b>
<pre>#!/bin/bash
chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv</pre>
<b>bandit21@bandit:/etc/cron.d$ file /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv</b>
<pre>/tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv: ASCII text</pre>
<b>bandit21@bandit:/etc/cron.d$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv</b>
<pre>Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI</pre></p>
<p> Password to next level is: Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI</p>

<h1> bandit 22 </h1>
<p><b>bandit22@bandit:~$ ls</b>
<b>bandit22@bandit:~$ cd /etc/cron.d</b>
<b>bandit22@bandit:/etc/cron.d$ cat cronjob_bandit23</b>
<pre>* * * * * bandit23 /usr/bin/cronjob_bandit23.sh  &> /dev/null</pre>
<b>bandit22@bandit:/etc/cron.d$ cat /usr/bin/cronjob_bandit23.sh</b>
<pre>#!/bin/bash
myname=$(whoami)
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)
echo "Copying password file /etc/bandit_pass/$myname to /tmp/$mytarget"
cat /etc/bandit_pass/$myname > /tmp/$mytarget</pre>
<b>bandit22@bandit:/etc/cron.d$ whoami</b>
<pre>bandit22</pre>
<b>bandit22@bandit:/etc/cron.d$ echo I am user bandit23 | md5sum | cut -d ' ' -f 1</b>
<pre>8ca319486bfbbc3663ea0fbe81326349</pre>
<b>bandit22@bandit:/etc/cron.d$ cat /tmp/8ca319486bfbbc3663ea0fbe81326349</b>
<pre>jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n</pre></p>
<p> Password to next level is: jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n</p>

<h1> bandit 23 </h1>
<p>check content of /etc/cron.d/:
<br><b>bandit23@bandit:~$cat /usr/bin/cronjob_bandit24.sh</b>
<pre>#!/bin/bash
myname=$(whoami)
cd /var/spool/$myname
echo "Executing and deleting all scripts in /var/spool/$myname:"
for i in * .*;
do
    if [ "$i" != "." -a "$i" != ".." ];
    then
	echo "Handling $i"
	timeout -s 9 60 ./$i
	rm -f ./$i
    fi
done
</pre></p>
<p>Creat your own folder to edit:
<br><b>bandit23@bandit:~$mkdir /tmp/hg </b>
<br>change to /tmp/hg/ then create your script: 
<br><b>bandit23@bandit:/tmp/hg$vi hg.sh  </b>
<pre><code>#!/bin/bash 
cat /etc/bandit_pass/bandit24 > /tmp/hg/hg.sh </code></pre></p>
<p><b>Important</b>: remember to change the permission of your script before copying it to the /var/spool/bandit24 folder or it will not be run by the bandit24 account. It took me a few tries to notice it.
<br>bandit23@bandit:/tmp/hg$ chmod 777 . hg.sh 
</p>
</p>copy this cript to <i> /var/spool/bandit24/</i>
<br><b>bandit23@bandit:/tmp/hg$ cp hg.sh /var/spool/bandit24</b>
<br>then check with <i> ls /var/spool/bandit24/</i>
<br> The scripts in /var/spool/bandit24 will be run once and then purged away every minute. 
<br><b>bandit23@bandit:/tmp/hg$ cat hg.sh</b>
<pre><code>UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ</code></pre>
</p>
<p> Password to next level is: UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ</p>

<h1> bandit 24 </h1>
create script to brute force pin code:
<br><b>bandit24@bandit:/tmp/hg$ cat brute_force.sh</b>
<pre>#!/bin/bash
for i in {1..10000}
do
 echo "UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ $i" >> ./out
done</pre>
<b>bandit24@bandit:/tmp/hg$ cat out | nc localhost 30002</b>
<p>Password to next level is: uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG</p>

<h1> bandit 25 </h1>
resize windows as small as possible then log in with ssh:
<br><b>bandit25@bandit:~$ ssh bandit26@localhost  -i bandit26.sshkey</b>
<br> when see <i>"More (%)"</i> type <b>v</b> then
<br><b>:set shell=/bin/bash
<br>:shell</b>
<pre>5czgV9L3Xx8JPOyRbXh6lQbmIOWvPT6Z</pre>
Password to next level is: 5czgV9L3Xx8JPOyRbXh6lQbmIOWvPT6Z

<h1> bandit 26 </h1>
just same bandit20
<br><b>bandit26@bandit:~$ ./bandit27-do cat /etc/bandit_pass/bandit27</b>
<pre>3ba3118a22e93127a4ed485be72ef5ea</pre>
Password to next level is: 3ba3118a22e93127a4ed485be72ef5ea

<h1> bandit 27 </h1>
try:
<br><b>bandit27@bandit:~$ git clone ssh://bandit27-git@localhost/home/bandit27-git/</b>
<pre>fatal: could not create work tree dir 'bandit27-git': Permission denied</pre>
then change to direcotry can write:
<br><b>bandit27@bandit:~$ cd /tmp/hg</b>
<br><b>bandit27@bandit:/tmp/hg$ git clone ssh://bandit27-git@localhost/home/bandit27-git/repo</b>
<br><b>bandit27@bandit:/tmp/hg$ cd repo</b>
<br><b>bandit27@bandit:/tmp/hg/repo$ ls</b>
<pre>README</pre>
<b>bandit27@bandit:/tmp/hg/repo$ cat README </b>
<p>The password to the next level is: 0ef186ac70e04ea33b4c1853d2526fa2</p>

<h1> bandit 28 </h1>
work again with git
<br><b>bandit28@bandit:/tmp/hg$ git clone ssh://bandit28-git@localhost/home/bandit28-git/repo</b>
<br>change into repo
<br><b>bandit28@bandit:/tmp/hg$ ls repo/</b>
<pre>README.md</pre>
<b>bandit28@bandit:/tmp/hg$ cat repo/README.md </b>
<pre># Bandit Notes
Some notes for level29 of bandit.

 credentials

- username: bandit29
- password: xxxxxxxxxx</pre>
<b>bandit28@bandit:/tmp/hg$ git log</b>
<pre>fatal: your current branch 'master' does not have any commits yet</pre>
<b>bandit28@bandit:/tmp/hg$ cd repo/</b>
<br><b>bandit28@bandit:/tmp/hg/repo$ git log</b>
<pre>commit 073c27c130e6ee407e12faad1dd3848a110c4f95
Author: Morla Porla <morla@overthewire.org>
Date:   Tue Oct 16 14:00:39 2018 +0200

    fix info leak

commit 186a1038cc54d1358d42d468cdc8e3cc28a93fcb
Author: Morla Porla <morla@overthewire.org>
Date:   Tue Oct 16 14:00:39 2018 +0200

    add missing data

commit b67405defc6ef44210c53345fc953e6a21338cc7
Author: Ben Dover <noone@overthewire.org>
Date:   Tue Oct 16 14:00:39 2018 +0200

    initial commit of README.md</pre>
<b>bandit28@bandit:/tmp/hg/repo$ git show HEAD</b>
<pre><code>commit 073c27c130e6ee407e12faad1dd3848a110c4f95
Author: Morla Porla <morla@overthewire.org>
Date:   Tue Oct 16 14:00:39 2018 +0200

    fix info leak

diff --git a/README.md b/README.md
index 3f7cee8..5c6457b 100644
--- a/README.md
+++ b/README.md
@@ -4,5 +4,5 @@ Some notes for level29 of bandit.
 ## credentials
 
 - username: bandit29
-- password: bbc96594b4e001778eee9975372716b2
+- password: xxxxxxxxxx</pre></code>
The password to the next level is: bbc96594b4e001778eee9975372716b2

<h1> bandit 29 </h1>
show content of README.md after clone:
<br></b>bandit29@bandit:/tmp/hg$ cat repo/README.md </b>
<pre><code># Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: <no passwords in production!></pre></code>
check other branch
<br><b>bandit29@bandit:/tmp/hg/repo$ git show-branch -a --list</b>
<pre>* [master] fix username
  [origin/HEAD] fix username
  [origin/dev] add data needed for development
  [origin/master] fix username
  [origin/sploits-dev] add some silly exploit, just for shit and giggles</pre>
try dev first:
<br><b>bandit29@bandit:/tmp/hg/repo$ git checkout dev</b>
<pre>Branch dev set up to track remote branch dev from origin.
Switched to a new branch 'dev'</pre>
<b>bandit29@bandit:/tmp/hg/repo$ ls</b>
<pre>code  README.md</pre>
<b>bandit29@bandit:/tmp/hg/repo$ cat README.md </b>
<pre><code># Bandit Notes
Some notes for bandit30 of bandit.

## credentials

- username: bandit30
- password: 5b90576bedb2cc04c86a9e924ce42faf
</pre></code>
The password to the next level is: 5b90576bedb2cc04c86a9e924ce42faf

<h1> bandit 30 </h1>
<b>bandit30@bandit:/tmp/hg$ cat repo/README.md </b>
<pre>just an epmty file... muahaha</pre>
<b>bandit30@bandit:/tmp/hg$ cd repo/</b>
<br><b>bandit30@bandit:/tmp/hg/repo$ git log</b>
<pre><code>commit 3aa4c239f729b07deb99a52f125893e162daac9e
Author: Ben Dover <noone@overthewire.org>
Date:   Tue Oct 16 14:00:44 2018 +0200

    initial commit of README.md
</pre></code>
 there no things can use, so try git remote:
<br><b>bandit30@bandit:/tmp/hg/repo$ git ls-remote</b>
<pre>From ssh://bandit30-git@localhost/home/bandit30-git/repo
3aa4c239f729b07deb99a52f125893e162daac9e	HEAD
3aa4c239f729b07deb99a52f125893e162daac9e	refs/heads/master
f17132340e8ee6c159e0a4a6bc6f80e1da3b1aea	refs/tags/secret
</pre>
let try tags:
<br><b>bandit30@bandit:/tmp/hg/repo$ git tag</b>
<pre>secret</pre>
<b>bandit30@bandit:/tmp/hg/repo$ git show-ref --tags -d</b>
<pre>f17132340e8ee6c159e0a4a6bc6f80e1da3b1aea refs/tags/secret</pre>
<b>bandit30@bandit:/tmp/hg/repo$ git cat-file -p f17132340e8ee6c159e0a4a6bc6f80e1da3b1aea</b>
<pre>47e603bb428404d265f59c42920d81e5</pre>
The password to the next level is: 47e603bb428404d265f59c42920d81e5

<h1> bandit 31 </h1>
<b>bandit31@bandit:/tmp/hg/repo$ cat README.md </b>
<pre>This time your task is to push a file to the remote repository.

Details:
    File name: key.txt
    Content: 'May I come in?'
    Branch: master
</pre>
just do it:
<br><b>bandit31@bandit:/tmp/hg/repo$ echo "May I come in?" > key.txt</b>
<br><b>bandit31@bandit:/tmp/hg/repo$ git add -f key.txt</b>
<br><b>bandit31@bandit:/tmp/hg/repo$ git commit -m "task"</b>
<pre>[master e0578da] task
 1 file changed, 1 insertion(+)
 create mode 100644 key.txt
 </pre>
<b>bandit31@bandit:/tmp/hg/repo$ git push</b>
<pre>Could not create directory '/home/bandit31/.ssh'.
The authenticity of host 'localhost (127.0.0.1)' can't be established.
ECDSA key fingerprint is SHA256:98UL0ZWr85496EtCRkKlo20X3OPnyPSB5tB5RPbhczc.
Are you sure you want to continue connecting (yes/no)? yes
Failed to add the host to the list of known hosts (/home/bandit31/.ssh/known_hosts).
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames
</pre>
<b>bandit31-git@localhost's password: </b>
<pre>Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 316 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
remote: ### Attempting to validate files... ####
remote: 
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote: 
remote: Well done! Here is the password for the next level:
remote: 56a9bf19c63d650ce78e6ec0354ee45e
remote: 
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote: 
To ssh://localhost/home/bandit31-git/repo
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'ssh://bandit31-git@localhost/home/bandit31-git/repo'</pre>
The password to the next level is: 56a9bf19c63d650ce78e6ec0354ee45e

<h1> bandit 32 </h1>
<b>>> sh</b>
<pre>sh: 1: SH: not found</pre>
<b>>> ls</b>
<pre>sh: 1: LS: not found</pre>
<b>>> ``
<br>>> ""
<br>sh: 1: : Permission denied</b>
<br>every character become upper key but symbols are not
<b>>> $0</b>
<pre>$ </pre>
<b>$ whoami</b>
<pre>bandit33</pre>
<b>$ cat /etc/bandit_pass/bandit33</b>
<pre>c9c3199ddf4121b10cf581a98d51caee</pre>
The password to the next level is: c9c3199ddf4121b10cf581a98d51caee

<h1> bandit 33 </h1>
<b>bandit33@bandit:~$ cat README.txt </b>
<pre>Congratulations on solving the last level of this game!

At this moment, there are no more levels to play in this game. However, we are constantly working
on new levels and will most likely expand this game with more levels soon.
Keep an eye out for an announcement on our usual communication channels!
In the meantime, you could play some of our other wargames.

If you have an idea for an awesome new level, please let us know!</pre>

<h1></h1>
