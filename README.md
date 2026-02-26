This is a small web app for doing weekly dinner planning using AI generated recipes.
It works against a Neo4j database, but you need to provide the Neo4j instance yourself and enter the credentials yourself in the UI. The Neo4j instance has to be 2026.02.0 or later and must be configured with CYPHER 25 or later as default language.

The front end part (HTML + Javascript) is vibe-coded around Cypher statements designed by me.
This explains why it is done in just one hugh index.html and why the structure is what it is :)

This is available as a web app here: https://christofferbergman.github.io/dinner-planner/

If you want to use this you need two things:
* An OpenAI API key
* A Neo4j instance

The first one has a cost, though it is not huge. You need to create an account on OpenAI and create an API key there.\
For the second one you can create an Aura Free instance in the cloud following these steps:\
1. Go to https://neo4j.com/ 
2. Click Get Started Free
3. Register and create an instance (select Free if you want to avoid costs)
4. Open your instance in the Query tool and execute this query: \
ALTER DATABASE neo4j SET DEFAULT LANGUAGE CYPHER 25
5. Store the instance URL and your password

Now you can use the URL, the password and the API key for the dinner planner tool. The user name and database should both be set to neo4j.

One thing to note if you use a Free instance is that it is paused if it isn't used for a few days, so you may need to login to your console and resume it before you can use the dinner planner. And if it isn't used for 30 days the data gets deleted (but you will be notified through email first).
