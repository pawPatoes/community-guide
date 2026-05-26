
# How to give moderator to any GDPS user 
* First login to panel and select your gdps.  
* Now, on the side, expand moderation section.  
* Select moderators/roles.  
* Now click create role and give yourself the perms you want   
* Afterwards, click add moderator, type in the username of user you want to add role to.  
* Now, In-game, go to settings > help > click req.
  
For manual import via [PHPMyAdmin](https://www.phpmyadmin.net/)
Here is a simple .sql that has the roles for you: [roles.sql](https://github.com/user-attachments/files/28278390/roles.sql)    
Simply import it inside of [PHPMyAdmin](https://www.phpmyadmin.net/)  
Heres how to do it manually:  
`(Some things were removed due to privacy, they aren't important to the tutorial)`  
<img width="291" height="476" alt="image" src="https://github.com/user-attachments/assets/3590c0e0-c1cd-42ac-bc92-796131c87f4d" />
<img width="1606" height="764" alt="image" src="https://github.com/user-attachments/assets/4ceb1b48-2cfe-477e-9a25-ffaada7fa65b" />
<img width="1551" height="770" alt="image" src="https://github.com/user-attachments/assets/26e43773-ff4d-4744-87c3-c4a3f1130735" />
<img width="1542" height="523" alt="image" src="https://github.com/user-attachments/assets/8240dac4-5ccc-4752-85de-b0b4c473c699" />  
Here you deleted the roles table, now follow these steps to add it back with the roles:  
<img width="1580" height="752" alt="image" src="https://github.com/user-attachments/assets/38cd8a35-00ec-49f9-a7c8-c7bdb93313fb" />
<img width="1535" height="680" alt="image" src="https://github.com/user-attachments/assets/f0a101cb-431d-42db-98a2-e3731a3492b2" />
<img width="1567" height="673" alt="image" src="https://github.com/user-attachments/assets/4b639ab3-7572-41ec-85a4-b1d17cfee2ba" />
<img width="1552" height="727" alt="image" src="https://github.com/user-attachments/assets/10b1fa61-b751-48f4-b438-ec8c7e17ef4c" /> 
Now the roles table has:  
* Owner (role id 1) Has all permissions.  
* Mod (role id 2) Can send levels and set demon difficulties.  
* Leaderboard Mod (role id 3) can run leaderboardsBan.php and leaderboardsUnban.php in (mod link)/tools.  
* Elder Mod (role id 4) can rate levels, can run !rate. Delete levels with !delete, and delete any comment or account comment.

How to assign these roles: `(Easy enough to follow without images)`
* Go to roleassign (Right ontop of roles).
* Go to the top bar and press "insert".
* Ignore assignID, don't touch it.
* AccountID is the account id of the person you wanna give mod, you can find this in the "accounts" table.
* RoleID is the role ids mentioned before.
* Press "Go".
* Then press "browse" in the top bar to see your changes.
* Now the person who got moderator (except leaderboard moderators, as they gain their powers instantly) can press the req. button in settings -> help -> req. to gain their powers!
