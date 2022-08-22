# aishwarydhare.github.io
After initiating the terraform run the terraform command : terraform validate, terraform plan, terraform apply
once the servers are up and running, enter into the server1
by that time you will find an file in /home/ubuntu/conf.d
Edit that file and input the belwo lines in that conf file 
     location /sample {
          proxy_pass http:// public Ip:5000/sample/;
       }
Then run the command : sudo docker cp ~/home/ubuntu/default.conf nginx-base:/etc/nginx/conf.d ( this command will copy the conf file of nginx in nginx dir ) 
