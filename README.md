# authentication-security-project

the second level of encryption is done by the mongoose encryption package. the encryption key is stored in .env file.


the third level of encryption is done through hashing. The process of hashing is done though md5 package from npm. Hashing is almost impossible to be reversed, which only comparing the login credential hashing result with the registered hashing password. It is theoretically safer than the basic level of encryption.  
