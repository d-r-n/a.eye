# HackTX-2020
## Inspiration
As virtual connections are becoming the norm today, meeting with people through video conferencing has become a staple of everyday tasks from work meetings to class presentations. Transitioning from everyday face-to-face interactions to video calls has presented its own unique challenges. We often feel like we are talking to computer screens, tiring our eyes by the constant exposure to screen light, neglecting to realize that real people are on the other side of the screen. As a result, our eyes tend to wander off, albeit unconsciously, and we lose focus in our meetings. Losing eye contact causes us to lose focus and engagement with our virtual audience. Therefore, our quotidian life of virtual video conferencing has inspired us to create a machine learning model that detects whenever our eyes gaze off the camera, and would signal an alert to us as a reminder to keep our focus in check. Our project, entitled a.Eye, is a play on the word "A.I" that leverages technology to help us keep an eye on our eye.

## What it does
The program will alert you with a notification when you are not making eye contact with the camera. 

## How we built it
1. Scrapped 4000+ photos from shutterstock.com of people looking at the camera and looking away from camera. 
2. Imported the pictures into AutoML on the Google Cloud. 
3. We labeled all the photos in AutoML. The photos of people looking at the camera were labeled "at camera" and the photos of people looking away from camera were labeled "not at camera"
4. We then trained the model on the 4000+ photos and deployed the model. 
5. Used the deployed model to create a python script that would notify someone if they were looking away from camera. 

## Challenges we ran into
We tried to do AutoML Vision API but it wasn’t working for us so we used AutoML Vision on Google Cloud. Our other problem was that the model we used took a long time to train since we used over 4,000 images. Having the model provide audio feedback when someone wasn't making eye contact was also a problem for us at first.

## Accomplishments that we're proud of
As a team of novices, this is our first time ever utilizing a cloud service, let alone build a full-scale machine learning model on it. After passing through multiple trial and errors, we have successfully built a model to detect whether or not you are looking at the camera with nearly 90% accuracy. On top of that, we built a real-time push notification system to alert you to look back at the camera if you gaze away and keep your focus. At the end of the day, we went from amateurs to believing that building a successful model with relevant application is not a dream, but rather something that could happen overnight.

## What we learned
On the technical side, we were able to familiarize ourselves with AutoML Vision on GCP. We have learned training 4000 images take around 4 hours but were able to get higher accuracy. It was definitely a trade-off that our group being patient paid off. We also were able to learn the importance of teamwork as we were able to get different insights and ideas which contributed to having the project in a better direction. In spite of the challenges, we were able to overcome the difficulties as a team.

## What's next for a.Eye
As we mentioned earlier, the virtual environment is developing and it is certain that this virtual environment will remain post-COVID. Our intention for the project is to have people to have a better experience interacting with others in the virtual settings so that at least they have a better chance to be more engaged. To have this project to be released to the real-world, we will try to first add this to the chrome extension. Every time the camera activates, this will activate at the same time so that it assists the user to make eye contact with the camera. 
