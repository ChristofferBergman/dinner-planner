This is a small web app for doing weekly dinner planning using AI generated recipes.
It works against a Neo4j database, but you need to provide the Neo4j instance yourself and enter the credentials yourself in the UI. The Neo4j instance has to be 2026.02.0 or later and must be configured with CYPHER 25 or later as default language.

The front end part (HTML + Javascript) is vibe-coded around Cypher statements designed by me.
This explains why it is done in just one hugh index.html and why the structure is what it is :)
