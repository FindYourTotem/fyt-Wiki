# Find Your Totem
[Marshall Briggs](https://github.com/marshdevs)<br>
[Rich Ung](https://github.com/RichUng)<br>
[Michelle Liu](https://github.com/michelleliu103)<br>
[Royce Duong](https://github.com/royceduong)<br>
Pierre Villanuevo

**About:**
This project was made for <a href="http://hacktilldawn.us/"> Hack Till Dawn</a> (Music festival themed hackathon hosted by Angelhack, sponsored by AWS and Intel) on May 5-6, 2018.

**Challenge:** Use AWS technology to create an experience that is desperately needed or would greatly enhance the fan experience at an EDC festival.

**Solution:** Use the AWS Deeplens and Console to detect festival totems and display their location on an app. ([video](https://vimeo.com/270776803))
![alt](https://s3-us-west-1.amazonaws.com/roycebucket1/fyt_stack.jpg)

# How It Works:
Under Construction. Last updated: June 25, 2018
## Activate Deeplens:
## Use Deeplens facial recognition model:
We used documentation from [@darwaishx](https://github.com/darwaishx)'s Github repo [Deep-Learning-With-Deep-Lens](https://github.com/darwaishx/Deep-Learning-With-Deep-Lens/tree/master/4-FaceDetectionAndVerification/1-FaceDetection) to crop faces and send them to an S3 bucket. 
* ### Crop Faces:
- ### Send images to S3 Bucket:  
    - Set up S3 Bucket.
    - Create IAM, give it permissions
    
## Take image from S3 and run AWS Rekognition API:
* Our [Lambda Function](
https://github.com/marshdevs/find-your-totem/blob/master/Lambda%20Functions/S3%20to%20Rekognition%20to%20End/lambda_function.py) event handler runs AWS Rekognition when a new photo is uploaded to the S3 bucket. If there is a match, it sends an object to our mobile app.

## Send to React Native Application:
* Display data on Application

---

> Without a license, all source code is copyright by default. You may read this code, but you have no legal 
> right to use it. To obtain usage rights, you must contact the author and request permission.

https://choosealicense.com/no-permission/
