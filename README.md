`Tryhackme  Simple_CTF`
--
By :- Unknownperson
-- 

## Port Scanning:-{21,80,2222}
>Than Also in 21 Port we got anonymous access in ftp port which contain file like this `/pub/ForMitch.txt`
> Which Content was :- `Dammit man... you'te the worst dev i've seen. You set the same pass for the system user, and the password is so weak... i cracked it in seconds. Gosh... what a mess!`
> Like there is Devloper Mitch who set very Weak Password In any System Login for Privilleged User

> After Directory Fuzzing We got Directory `/simple`
	>Which is CMD Simple 
> Than we got simple CMS vurnability for SQLijection `46635.py`
> Throw This We get Inintial Username And Password 
> In the Webserver we got Simple Apache webserver Page than we find get robots.txt Which Contain Username = `mitch`

# Credential :- `m**ch:s***et`

# Privillage Escalation

> Let first Check `sudo -l`
> Wow We got the direct sudo access run commmand of /usr/bin/vim

`sudo /usr/share/vim -c ':!/bin/sh'`
--

> Woww We got Root Access And We are the Admin

`
# At this way We Again Pawnd A Machine
`


-> Also `Disallow: /openemr-5_0_1_3` Entry Get
