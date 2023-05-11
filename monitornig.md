 MONITORING

(checking our services is working or not )getting o know about the problems
* now lets try to figure out any failure
    * network failure
    * harware "
    * application "

![preview](./Images/1.png)


 suppose you are assigned to figure out failures . to slove the issues we wil figureout a proactive approach
    for every one min.
    check if every server is responding or not
    check if application is responding or not
    alert if the servers or applications are not responding

logs: log is a record which specify some activity done 

* OS have log we might need to  finetune it
        windows = event viewer
        linux= syslog
* application also log try to uderstand about failure
 * log debug: to findout the errors in the logs(logs will appreare)
 * log info :  checking the logs whether it's present or not


* TRACING:
  it's an approch to figure out the flow of your system
  every s/m has resource utilization informations
        * cpu
        * memory
        * disk
        * network
METRICS:

  metrics are the values which reprasents some information about s/m
  or application with value as number with time dymention(x-axis time, y-axis value)

  * for example we can the qtinfo s/m need to monitoring the solutions we need to get (logs , metric, trace)
  * MTTR: mean time to recover(avarage time taken by ur organization to       recover from failures)
  * MTTF: meantime to fail (avg time during the certain toget an failure in ur s/m)
    * SLA: service level agriment(this is an agriment b/w service provider and customer w.r.t  availability and other importent metricks)
  
  . monitoring are two types 
      1. wight box monitoring
      2. block box monitoring

![preview](./Images/2.png)

(Request) Rate - the number of requests, per second, you services are serving.
(Request) Errors - the number of failed requests per second.
(Request) Duration - distributions of the amount of time each request takes

The resulting USE Method-derived checklists for different operating systems are listed on the left navigation panel (Linux, Solaris, etc). You can customize these for your environment, adding additional tools that your site uses. 

Monitoring
Collecting, processing, aggregating, and displaying real-time quantitative data about a system, such as query counts and types, error counts and types, processing times, and server lifetimes.

White-box monitoring

Monitoring based on metrics exposed by the internals of the system, including logs, interfaces like the Java Virtual Machine Profiling Interface, or an HTTP handler that emits internal statistics.

Black-box monitoring

Testing externally visible behavior as a user would see it.

latency: quick responce time(latency high responce low)
traffic: how many public or requests with your application 
errors: how many requests generally failed
saturation: what you are missed percentage 
  ex:  flipcart bigbilion days
utilization: what would have to done
   saturation is inversly praportional to utlization
database: to store the information >> memory files >> RAM

tread:

![images](./Images/3.png)

thread create adresses limit to acces user to applications 
treads also get a memory major preriy is CPU
 
load/stress testing : when from my s/m is not working  to check we use load testing (to figure out the saturation points)

monitoring are basically depends two types of data
  1.number(ex: what's our cpu and RAM utilizaion)
      system
      applications
  2.text/data (ex: why our system going solw performance)

Dashboard: complete application in one space
elastic strag: present every where

 monitorning/ obsorvability: 

####  Monitor typesedit
You can configure Heartbeat to use the following monitor types:

#### icmp
Uses an ICMP (v4 and v6) Echo Request to ping the configured hosts. Requires special permissions or root access.
#### tcp
Connects via TCP and optionally verifies the endpoint by sending and/or receiving a custom payload.
#### http
Connects via HTTP and optionally verifies that the host returns the expected response. Will use Elastic-Heartbeat as the user agent product.
browser
Allows users to run the synthetic monitoring tests via Synthetic Agent on the Chromium browser.
The tcp and http monitor types both support SSL/TLS and some proxy settings.

 


