# JWT

To help prepare for API authentication tomorrow, research [JSON Web Tokens](https://jwt.io) (known as JWTs). This should take about 30 minutes. Answer the following questions and submit this README as your homework:

1. What are the 3 parts of a JWT?

	1. a 'header'

	2. a payload

	3. a signature

2. What information does each part contain?

	1. The header contains two items
		-the algorithm used to hash the data or rather an abbreviation or key to identify that algorithm
		-as well as a file type identifier 'jwt'
	
	2. The payload contains the 'data' otherwise known as the claims, that the user or site would seek to 		send and receive.

	3. The signature contains the header and the payload, as well as a secret key as base64url encoded 		information that is then concatenated with periods leaving a long and seemingly random looking 		string of numbers, letters and periods.

3. Why do people use JWTs for authentication? A great resource to read would be https://jwt.io/introduction/.
	
		JWTs are often used in place of cookie authentication as a stateless form of authentication where the user's 'info' is never actually stored on a server and is simply used as a mechanism to allow the user to access the correct routing in order to access portions of the site, dba, api, or whatever they seek to gain access to. In doing this it protects the user from having their sensitive information stored anywhere but locally and also speeds up the process of authentication as it now becomes part of accessing the site rather than querying a server everytime for a key to gain access.