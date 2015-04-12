bandit wargame
==============
http://overthewire.org/wargames/bandit/

Level 0
-------
http://overthewire.org/wargames/bandit/bandit0.html

Level 0-1
---------
http://overthewire.org/wargames/bandit/bandit1.html

###helpful:###
http://linux.about.com/od/commands/l/blcmdl1_ssh.htm
exit - terminate ssh session

###commands:###
ssh bandit0@bandit.labs.overthewire.org
password: bandit0
ls
man cat
cat readme
	boJ9jbbUNNfktd78OOpsqOltutMc3MY1

Level 1-2
---------
http://overthewire.org/wargames/bandit/bandit2.html

###commands:###
ssh bandit1@bandit.labs.overthewire.org
	password: boJ9jbbUNNfktd78OOpsqOltutMc3MY1
ls
cat ./-
	CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

Level 2-3
---------
http://overthewire.org/wargames/bandit/bandit3.html

###commands:###
ssh bandit2@bandit.labs.overthewire.org
	password: CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
ls
cat ./spaces\ in\ this\ filename
	UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

Level 3-4
---------
http://overthewire.org/wargames/bandit/bandit4.html

###commands:###
ssh bandit3@bandit.labs.overthewire.org
	password: UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
ls
cd inhere
ls -lah
cat .hidden
	pIwrPrtPN36QITSp3EQaw936yaFoFgAB

Level 4-5
---------
http://overthewire.org/wargames/bandit/bandit5.html

###commands:###
ssh bandit4@bandit.labs.overthewire.org
	password: pIwrPrtPN36QITSp3EQaw936yaFoFgAB
ls
cd inhere
ls -lah
cat ./-file*
	koReBOKuIDDepwhWk7jZC0RTdopnAYKh

Level 5-6
---------
http://overthewire.org/wargames/bandit/bandit6.html

###commands:###
ssh bandit5@bandit.labs.overthewire.org
	password: koReBOKuIDDepwhWk7jZC0RTdopnAYKh
find . -type f -size 1033c -exec '{}' \;
cd inhere/maybehere07/
cat ./.file2
	DXjZPULLxYr17uwoI01bNLQbtFemEgo7

Level 6-7
---------
http://overthewire.org/wargames/bandit/bandit7.html

###commands:###
ssh bandit6@bandit.labs.overthewire.org
	password: DXjZPULLxYr17uwoI01bNLQbtFemEgo7
find / -group bandit6 -user bandit7 -size 33c ! -executable
cat /var/lib/dpkg/info/bandit7.password
	HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs

Level 7-8
---------
http://overthewire.org/wargames/bandit/bandit8.html

###commands:###
ssh bandit7@bandit.labs.overthewire.org
	password: HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
ls
grep millionth data.txt
	cvX2JJa4CFALtqS87jk27qwqGhBM9plV

Level 8-9
---------
http://overthewire.org/wargames/bandit/bandit9.html

###commands:###
ssh bandit8@bandit.labs.overthewire.org
	password: cvX2JJa4CFALtqS87jk27qwqGhBM9plV
ls
sort data.txt | uniq -u
	UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR

Level 9-10
---------
http://overthewire.org/wargames/bandit/bandit10.html

###commands:###
ssh bandit9@bandit.labs.overthewire.org
	password: UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
ls -lh
strings data.txt | grep -e "^=.*$"
	truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk

Level 10-11
---------
http://overthewire.org/wargames/bandit/bandit11.html

###commands:###
ssh bandit10@bandit.labs.overthewire.org
	password: truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk
base64 -d data.txt | less
	IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR

Level 11-12
---------
http://overthewire.org/wargames/bandit/bandit12.html

###commands:###
ssh bandit11@bandit.labs.overthewire.org
	password: IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR
strings data.txt | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'
	5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu

Level 12-13
---------
http://overthewire.org/wargames/bandit/bandit13.html

###commands:###
ssh bandit12@bandit.labs.overthewire.org
	password: 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu
mkdir /tmp/ig21
cd /tmp/ig21
xxd -r ~/data.txt > /tmp/ig21/data
file data
mv data data.gz; gzip -d data.gz
ls -lh
file data
mv data data.bz; bzip2 -d data.bz
ls -lh
file data
mv data data.gz; gzip -d data.gz
ls -lh
file data
mv data data.tar; tar -xvf data.tar
ls -lh
rm data.tar
mv data5.bin data.tar; tar -xvf data.tar
rm data.tar
file data6.bin
mv data6.bin data.bz; bzip2 -d data.bz
ls -lh
file data
mv data data.tar; tar -xvf data.tar
rm data.tar
file data8.bin
#	file -i data8.bin
mv data8.bin data.gz; gzip -d data.gz
ls -lh
file data
less data
	8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
#	Cleanup
cd ~
rm -r /tmp/ig21

Level 13-14
---------
http://overthewire.org/wargames/bandit/bandit14.html

###commands:###
ssh bandit13@bandit.labs.overthewire.org
	password: 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL
ls -lh
	sshkey.private
nmap localhost
ssh -i sshkey.private bandit14@127.0.0.1
file /etc/bandit_pass/bandit14
less /etc/bandit_pass/bandit14
	4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

Level 14-15
---------
http://overthewire.org/wargames/bandit/bandit15.html

###commands:###
ssh bandit14@bandit.labs.overthewire.org
	password: 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
nmap localhost
telnet 127.0.0.1 30000
	4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
	BfMYroe26WYalil77FoDi9qh59eK5xNr

Level 15-16
---------
http://overthewire.org/wargames/bandit/bandit16.html

###commands:###
ssh bandit15@bandit.labs.overthewire.org
	password: BfMYroe26WYalil77FoDi9qh59eK5xNr
nmap localhost
openssl s_client -connect localhost:30001 -quiet
	BfMYroe26WYalil77FoDi9qh59eK5xNr
	cluFn7wTiGryunymYOu4RcffSxQluehd

Level 16-17
---------
http://overthewire.org/wargames/bandit/bandit17.html

###commands:###
ssh bandit16@bandit.labs.overthewire.org
	password: cluFn7wTiGryunymYOu4RcffSxQluehd
nmap -A -p 31000-32000 localhost
	
	Starting Nmap 5.21 ( http://nmap.org ) at 2014-07-30 09:10 UTC
	Nmap scan report for localhost (127.0.0.1)
	Host is up (0.0011s latency).
	Not shown: 995 closed ports
	PORT      STATE SERVICE VERSION
	31000/tcp open  ssh     OpenSSH 5.9p1 Debian 5ubuntu1.4 (protocol 2.0)
	31046/tcp open  echo
	31518/tcp open  msdtc   Microsoft Distributed Transaction Coordinator (error)
	31691/tcp open  echo
	31790/tcp open  msdtc   Microsoft Distributed Transaction Coordinator (error)
	31960/tcp open  echo
	Service Info: OSs: Linux, Windows

	Service detection performed. Please report any incorrect results at http://nmap.org/submit/ .
	Nmap done: 1 IP address (1 host up) scanned in 41.38 seconds

mkdir /tmp/ig21
cd /tmp/ig21

openssl s_client -connect localhost:31790 -quiet > bandit17.private
	depth=0 CN = localhost
	verify error:num=18:self signed certificate
	verify return:1
	depth=0 CN = localhost
	verify return:1
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

	read:errno=0
ls -lh
chmod a-rw,u+rw bandit17.private
ssh -i bandit17.private bandit17@127.0.0.1

Level 17-18
---------
http://overthewire.org/wargames/bandit/bandit18.html

###commands:###
	!Must be logged in as bandit16!

