# alb_with_https_traffic_using_self_signed_cert

Steps:
======
1. Create ALB and Target Group
2. Create launch config 
3. Create ASG with launch config and attached ALB to it.
4. Create a self signed certificate
5. Now create new https listener for our existing alb and attached certificate created in above step.


For Step 1,2,3 Follow the attached document.

4. Create a self signed certificate and import it into ACM.

https://github.com/tushardashpute/generating-self-signed-certificate.git

5. Create new https listener for our existing alb and attached certificate created in above step.
