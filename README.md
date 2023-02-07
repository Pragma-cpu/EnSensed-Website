# EnSensed-Website
Website link: https://csi-annotation.web.app/


# Frontend structure


## index.html
Basic homepage
## signin.html*
Sign in page for registered users 
## signup.html*
Registration page for new users 
## viewFast.html*
The page displays a random video from our in-house dataset. A toggle button can be used by the annotator to idicate whether the person in the video is engaged or not. They can save the response by clicking the "save" button and click the "Find Next Video" to get the new video for annotation. They may click the video name to play it or click the "Find Next Video" button again to get another video.  The page displays the number of videos left in the database and the number of videos annotated by the user.
## about.html
Displays the project details.
## people.html
Displays the naems of the team members.


(*) Please add your firebase config details (under project overview) to the .html files. 


# Backend structure
* annotatorDetails  
&ensp; <user_email>  
&ensp;&ensp; age  
&ensp;&ensp; country  
&ensp;&ensp; gender  
&ensp;&ensp; profession  
  
* csi-annotation  
&ensp; <user_email>  
&ensp; &ensp; <video_name>  
&ensp;&ensp; &ensp; annotation: 0/1 

* videoCount  
&ensp; <video_name>  
&ensp; &ensp; count: 0/1/2/3  (if 3 videoPresent-><video_name> is removed )

* videoPresent 
&ensp; <video_name>  
&ensp; &ensp; present: 1 (iniial)


  


  
