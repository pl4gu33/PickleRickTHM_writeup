# PickleRickTHM_writeup

<h2> 1. Use NMAP to check on the opened ports <h2>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/1.png width="500" title="1"></img>
<h5> As we can see we have 2 open ports (22, 80) (ignore the activate windows plz) 🥲 </h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/2.png width="500" title="1"></img>
<h5> Now lets check what the website (hint: the source code) </h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/3.png width="500" title="1"></img>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/4.png width="500" title="1"></img>
<h5> As we can see there it is the username commented out in the source code </h5>
<h5> Looking back at the gobuster output we can see "robots.txt", lets paste that on our passw.. it worked! </h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/5.png width="500" title="1"></img>
<h5> As we can see in the website we have a command panel, lets type any commands to see if it works.. it does work!</h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/6.png width="500" title="1"></img>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/7.png width="500" title="1"></img>
<h5> We can see the "Sup3rS3cretPickl3Ingred.txt" lets paste it in the browser since the cat command is disabled, there is our first ingredient </h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/8.png width="500" title="1"></img>
<h5>Lets check what directory we are on now</h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/9.png width="500" title="1"></img>
<h5>Lets move to the home directory and check the users</h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/10.png width="500" title="1"></img>
<h5>We can see there is a user named rick, lets move to it. There is our second ingredient!</h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/11.png width="500" title="1"></img>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/12.png width="500" title="1"></img>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/13.png width="500" title="1"></img>
<h5>Let us check the user permissions using "sudo -l"</h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/14.png width="500" title="1"></img>
<h5>We can see that we can execute any command without any password. Since that is the case, lets sudo to root </h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/15.png width="500" title="1"></img>
<h5>We can see a txt file lets use the less command to see its contents.. :)</h5>
<img src=https://github.com/pl4gu33/PickleRickTHM_writeup/blob/main/img/16.png width="500" title="1"></img>
<h4>thats it for the walkthrough for pickle rick. make sure you follow my github for future scripts projects etc</h4>
