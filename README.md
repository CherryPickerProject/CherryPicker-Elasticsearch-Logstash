# CherryPicker-Elasticsearch-Logstash

- This project contains the configuration file to sync data from MongoDB Atlas to Elasticsearch cluster hosted on AWS.

1. Please obtain the .env file before running.
2. If using on a new EC2, Transfer your project folder to ec2 using FileZilla

   Add your .pem file to fileZilla

   setting>connection>SFTP

   file>SiteManager>(key in your ec2 endpoint)

3. If using on a new EC2, export the environment variables

`export ELASTIC_SEARCH_ENDPOINT=<endpoint>`

`export ELASTIC_AWS_ACCESS_KEY=<accesskey>`

`export ELASTIC_AWS_SECRET_KEY=<secretkey>`

`export MONGODB_CONNECTION_STRING=<mongo connection string>`

- Intended to run the following commands
- Change Directory `cd ~`

- Run config file `../../usr/share/logstash/bin/logstash -f ~/CherryPicker-Elasticsearch-Logstash/logstash.conf`
