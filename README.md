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

<img width="993" alt="image" src="https://user-images.githubusercontent.com/74225291/176090751-110d946a-070a-4ff7-a0cd-5de91c14caa0.png">

Till now we can access the ALB using http only, now we can add https listener to the ALB we created and attached certificate.

<img width="1108" alt="image" src="https://user-images.githubusercontent.com/74225291/176091108-9fdcfae8-7be4-4146-b0a5-c259c8ee677e.png">

Click on Add listener.

<img width="1006" alt="image" src="https://user-images.githubusercontent.com/74225291/176091183-560d4f48-3e53-4563-b503-8ed6d511c6b8.png">

Select newly created ACM.

<img width="1029" alt="image" src="https://user-images.githubusercontent.com/74225291/176091269-302b1ab5-90f8-4abe-b90d-afe892d5accb.png">


<img width="949" alt="image" src="https://user-images.githubusercontent.com/74225291/176091296-ec456ad3-64da-4112-be25-f49acf19ac31.png">


<img width="1216" alt="image" src="https://user-images.githubusercontent.com/74225291/176091343-7791bd4d-0ab1-4aef-87cc-048f74c636f3.png">


Now we can access traffic on https.


