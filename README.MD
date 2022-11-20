LOCUST IS USED TO GENERATE LOAD FOR APPLICATION AND SEE PERFORMANCE

Step1: DEPLOY KUBERNETES LOCUST

#git clone https://github.com/gauravkumar9130/kube-performance.git
#cd kube-performance
#kubectl create -f .

Step 2: Open Kubernetes Locust

#kubectl get services
COPY PUBLIC IP OF locust-service AND OPEN ON BROWSER WITH PORT NUMBER 8089

Step 3: Deploy Sample Application

#git clone https://github.com/gauravkumar9130/monolith
#cd monolith
#kubectl create -f .
#kubectl get pods
#kubectl get svc

Step 4: Generate Load For Sample Application

Go to Locust Console:
Number of Users: 10000		##HOW MANY TOTAL REQUESTS WANT TO SEND		
Spawn Rate: 100			##HOW MANY USER REQUESTS WILL GO PER SECOND
Host: IP OR DOMAIN WHERE WE WANT LOAD		##TARGET HOST
Run Time: 1h 					##TIMEOUT

With above example it will send total 10000 request and every second it will 100 requests, It will automatically close after 1 hour.


