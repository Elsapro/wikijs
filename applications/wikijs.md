<!-- TITLE: Wiki.js -->
<!-- SUBTITLE: A quick summary of Wiki.js -->

# Wiki.js
## Evaluation
I spend some time play with WIKI.JS and read the documetation. Here is my comments:
WIKI.JS is base on NodeJS, store metadata in MongoDB and store files in file system which can sync with Github. 
Features I like:
	• Social authentication integration: Google, Facebook, Microsoft
	• Third-party storage: User can choose the storage service they trust.
	• Moden UI. 
	• Support Markdown authoring. (Do you know if you put markdown file into Github, it can directly convert to HTML and display?)
	• There is already more than 10 languages supported. 
The gap with what I think:
	• No concept of version and history. (In the plan but not yet support)
	• Documentation is poor
	• The technical stack does not align with us. 
		○ We were using Java (SSH) to build the system. In next version, I plan to using Sprint Boot. (www.sprint.io)
		○ Java is mature to process XML. I see there are also libraries to process markdown. 
	• The plan is to replace MongoDB with other mechanism. See the following:
		○ MongoDB is being phased out in favor of PostgreSQL/MySQL/MSSQL/SQLite + Redis. An upgrade tool will be provided to migrate existing data to the new system.
I think this product is still in early stage. Features are still under development and documetation is still poor. I think there are still way to go for them. 
See the milestone list here:
https://github.com/Requarks/wiki