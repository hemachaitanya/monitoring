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
     
