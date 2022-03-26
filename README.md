# authentication-security-project

the second level of encryption is done by the mongoose encryption package. the encryption key is stored in .env file.


the third level of encryption is done through hashing. The process of hashing is done though md5 package from npm. Hashing is almost impossible to be reversed, which only comparing the login credential hashing result with the registered hashing password. It is theoretically safer than the basic level of encryption.  


the fourth level of encryption is thourgh the bcrypt.js. Originally, the course is asking to use node.bcrypt.js, but it seems deprecated. As suggested in the comment,  bcrypt.js is used. One issue did occur was that during second level of encryption, I used same testing email address, which resulted an issue when trying to compare the login info. It has successfully logged me in somehow. It should be figured it later. Adding a salt to hash made it time costly to hack, which would make the hacker to lost interest on doing such thing. If the do, that would be a waste of their computing power. The time of salt used is 10. 


The fifth level is using passport.js. It provides a more mature way for authentication. Express-session is also used. Cookies has been used to keep used logged in.
