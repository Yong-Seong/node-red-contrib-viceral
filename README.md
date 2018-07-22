# Build

From git repo dir
* npm install
* cd vizceral-example 
* npm install
* ./node_modules/.bin/webpack 
* npm run copy:fonts
* npm run copy:json


# Run 
From github repo dir
* ./start


# Details
Base URL to see viceral
* http://localhost:1880

Admin URL
* http://localhost:1880/admin
	userid: admin
	password: admin
        See node-red security on how to change the password

Search Endpoint
* http://localhost:1880/query-elasticsearch


# Extra info

The Simple and Complex static data should work right out of the box
For elasticsearch you will have to do the following
* For elasticsearch you have to go to the Elasticsearch Flow tab
* edit the ElasticSearch Webservers node and add your ELK and index information
* Then you have to review the Search Webtier node and change to your desire
I have all my apache logs parsed for "type: apache" host, respone_code, host_ip(you may have host) vhost field  
* WARNING don't change the aggregation bucket names then you will have to modify the Javascript later on, and i can tell you that will be a pain

 
