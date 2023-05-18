first we create 2 instances 
in one instance we install heart beat
onther install we install apache2 or nginx
we create elastic cloud account  with name ()in deployment 
save that credencials of elastic cloud password and cloudid
 * in heart-beat  
    whereis heartbeat.yml
    cd /etc/heartbeat/heatrtbeat.yml
    id:
    name:
    port: http://localhost:80
    enable: true
    
    elastic cloud
    * cloud id :
      cloud auth:

* go to the elastic cloud 
    goto kibana
    home- uptime
    createrule - monitor status rule - context.monitorname 

### grok debugging

[referedlink](https://grokdebugger.com/)

log messages will be split into some lowlevel understanding is called deugging by using grok s/w
### ex:
  8:45 AM 5/18/2023 INFO user Login Success
  8:45 AM 5/18/2023 INFO ERROR User Not Found
  8:45 AM 5/18/2023 INFO user Logout 

  (?<date>\d+:\d+\s+[AaPp][Mm]\s+\d+/\d+/\d+)%{SPACE}%{LOGLEVEL:level}%{SPACE}%{GREEDYDATA:message}

  o/p:
  [
  {
    "date": "8:45 AM 5/18/2023",
    "level": "INFO",
    "message": "user Login Success"
  },
  {
    "date": "8:45 AM 5/18/2023",
    "level": "INFO",
    "message": "ERROR User Not Found"
  },
  {
    "date": "8:45 AM 5/18/2023",
    "level": "INFO",
    "message": "user Logout Success"
  }
  ]
  ### EX:
   


     
