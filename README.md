# S3-Pre-signed-URLs
A pre‑signed URL embeds a cryptographic signature (Signature V4) granting specific access to a private S3 object (e.g., GET or PUT). It’s valid only for a limited time and is authenticated via query parameters 

Step 1 : Go to aws management console and navigate to S3 dashboard.

Step 2 : Create a s3 bucket having no public access and then upload an object in it.

Step 3 : copy the object URL and paste on the browser .It will show you access denied .This is because this object is private (not public).
Step 4 : but when you try to access it using “open” button in object ,the object will open this is because of presigned url.but this url is not applicable for the user other than aws account user.

Step5 : pre-signed urls are basically the urls which allows the access of private objects to any user which has a presigned url of the object but only for a limited time period which you set during the creation of the pre-signed url.

Step 6: Now to create a pre-signed url ,click on the object that you want to share and then go to  “object action” and then click on “share a pre-signed url” .
Step 7: then specify the time period for till when  you want to activate your object url .After the selected time period lets say after 5 minutes ,the pre-signed url will be deactivate.here we select the time period for 3 minutes.
Step 8: specify the time and click on “create presigned url” and then copy the url and after that paste that url in any browser with email different from your aws account or share the url to your friend and ask to open ,it will be accessible to all but until 3 minutes.

Step 9: So this is how a pre-signed url works!! 
