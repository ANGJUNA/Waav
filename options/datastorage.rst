4. Data Storage
=============
   * MySQL8.0 - Currently being used. In production, it's in AWS RDS server 
     and running on very expensive machine

   * Handling Terabytes of Data [Can’t imagine to dump the whole production database 
     to any development or local environment. Only way is to get the data structure 
and to some extent, a copy of live data in few tables]
   
   * TODO: NEED to link with HOW TO SETUP in LOCAL readme of git (branch name: local) 
Under modification / Development
   
   * For Development, local setup is being used and connected the local mysql as because 
of legacy code LATENCY is greatly multiplied in most of the pages due to multiple 
mysql protocol communication with remove RDS server. If client (waav application) 
is in AWS server, the latency is in range of 2 ms but if in other web network 
location, getting multiplied by tens or hundreds. End result, most of the waav 
pages in current legacy code takes minutes to load if connected to remote (copy or production) server.
