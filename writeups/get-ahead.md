GET aHEAD
Description
Find the flag being held on this server to get ahead of the competition: http://mercury.picoctf.net:4503/

Solution
I used Burp Suite to solve this challenge. First, I intercepted the request and sent it to the Repeater.

Then, I changed the GET request to a HEAD request. In the response headers, I found the flag.

Flag: picoCTF{r3j3ct_th3_g3t_r3qu3st_f6696225}
