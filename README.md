# How To Make Your Own Quarantine Wedding AR Filter

# #Introduction:
In this tutorial, you will be learning how to use Spark AR to create your own AR Filter using Head Occluder and 3D Objects.   Covid-19 has changed the way we interact as a community.  With this AR filter, you can allow people to be part of the event without actually being there.  Your friends and family that can’t make it can utilize this filter and share on their Instagram. 
 
## You will learn:
Downloading and setting up Spark AR Studio
Creating and modifying a head tracking project
Adding objects and animations
Utilizing the Head Occluder
Putting all together to make the filter

This tutorial is for complete beginners and just assumes you have access to a computer that can run Spark AR.  Not required, but nice to have would be pre existing digital objects that you want to incorporate into your filter.  

## Getting Started:

In order for this to work best, you can create your own 3D object.  This tutorial assumes you already have a 3D object or that you will be using one of the built in assets available in Spark AR Studio.  If you want to create your own 3D asset, you can do so in either Tinkercad.com or by using Paint 3D in Windows 10.  This entire tutorial can be done using default assets, but for the best effect, you’ll want to bring in your own 3D objects.  

### Step 1: Download Spark AR Studio

Go to https://sparkar.facebook.com/ar-studio
Click on Download on the top right corner, pink button.

Then click on the next pink button that says Download. 


And that’s it.  Depending on your internet connection, it will take a few minutes to download.  Now, let’s install the software!


### Step 2: Installing Spark AR Studio

Click on the downloaded image called SparkARStudio_v98.msi.

Follow the instructions to install. Click on Next.


Read and accept terms in the License Agreement. Click on Next. 


Follow special instructions for iOS users. Click Next. 




This screen is just to keep older versions of Spark AR Studio on your computer. Check the box if that is what you want to do. Then click on Next.


Choose where you want the program to be installed. Click on Next. 



Finally, click on Install. Note: you might get a pop-up window that says that this installation will change some devices. Click on Yes, then it will finish installing. 


Now that you have the software installed, it’s time to roll up your sleeves and start creating.  This tool is super powerful and there’s a lot going on.  


### Step 3: Starting your first project

Open Spark AR Studio and log in.
Click on New Project. 


 On the pop-up screen select Blank Project.








 Click on + Add Object, located in the The Scene panel, top left section of screen. 

 On the pop-up select Face Tracker and then click on the Insert button. 







 Right click on faceTraker0, located in The Scene panel, top left section, go to Add → Null Object.





This will add the item below to The Viewport.


 Right click on faceTraker0, located in The Scene panel, top left section, go to Add → Plane.

This will add the checker box to The Viewport.


 Drag plane0, located in The Scene panel, into nullObject0. It should look like this. 



9.  On the top menu, click on View → Show/Hide Patch Editor
 


### Step 4: Adding the Animation Loop

 With plane0 selected, right click in the Patch Editor, select Animation --> Loop Animation and then click on the button Add Patch.


A Loop Animation block should show in the Patch Editor.



 With plane0 selected, right click in the Patch Editor, select Animation → Transitions then click on the button Add Patch.


A Transition block should show in the Patch Editor.



 Select the nullObject0, located in The Scene panel, top left side of screen. In the The Inspector on the right side of the screen, click on the arrow in front of Rotation. This will turn the Rotation section yellow as shown below and a yellow block will appear in the Patch Editor. Link the Transition block to the Rotation block by clicking on the arrow located at the end of the Transition block and connecting it to the arrow in front of the Rotation block.  



 In the Transition block change the End values to x = 0, y = 360, and z = 0. This change will make the checker box speed in front of the person’s face. 


 In the Loop Animation block change Duration to 5. This change will make the checker box spin slower. 
 

 Select plane0, located in The Scene panel, top left side of screen. Then set  Z = 0.1 for the Position, located in The Inspector,  on the right side of the screen. This change will make the checker box spin and go around in front of the person’s face. Make the plane0 invisible by unchecking Visible on the Properties menu on The Inspector, right side of the screen. This will make the checker box disappear. 
 

### Step 5: Working with Head Occluder 

 Now we need the Head Occluder. To get the Head Occluder go download the Head Occluder from https://sparkar.facebook.com/ar-studio/learn/articles/people-tracking/face-reference-assets#whats-included-in-the-face-reference-assets 
Click on Download the Face Reference Assets here.

 A zip folder will be downloaded to your computer. Unzip the folder wherever you would like to save the content of the zip folder. In the The Assets panel, bottom left of screen,  click From Computer. Browse to the location where you unzip your download. Open headOccluder.obj. In my case I saved mine to my documents at C:\User\Documents\FaceAssets\Mesh\headOccluder.obj



The Assets panel, should look like this. 


 Add another Face Tracker to The Scene panel, top left of screen, you should have two face trackers now. Click on + Add Object → Face Tracker → Insert. 



 Right click on faceTraker1, then Add → Face Mesh.


You should now see a checker pattern on the face of the person. Like this. 




 Drag the headOccluder object in The Assets panel, bottom left section, to the faceTraker1 object, in The Scene panel, top left section. 


This is what you will see in The Viewport. 




 With the headOccluder selected go to the The Inspector, located on the right side of screen, change Scale to X = 0.19, Y = 0.19, Z = 0.19. Play around with those values they may vary from screen to screen. It has to be larger than the human head, but not too big. 


 Delete from The Assets panel, bottom left of screen, DefaultMaterial. Right click on DefaultMaterial then select Delete.


 In The Assets pane, located at the bottom left of screen, add an asset by clicking on + Add Asset and click on Material. You may rename it if you want, for the purpose of this tutorial this material will be named newMaterial. 


 With newMaterial selected in the The Assets panel, go to The Inspector, right side of screen and change Shader Type to Flat. 


The figures should look like this. 



 Select faceMesh0 under faceTracker1 on the The Scene panel, then in The Inspector, right side of screen, add newMaterial to Materials by clicking the plus sign and selecting newMaterail. 





 Select defaultobject under headOccluder in The Scene panel, top left side of screen. In The Inspector, the right side of the screen, change Material property to newMaterial. 


 In The Assets panel, bottom left of screen, select newMaterial. In The Inspector, the rightside of the screen, change the Opacity to 30 to be able to see the person's face. This will change later to 0 (zero).






 Select plane0 under faceTracker0 → nullObject0 → plane0 in The Scene panel, top left side of screen. In The Inspector, on the right side of the screen, check the Visible box to make the plane0 visible. 
 

The image of the person should look like this. 






 To make the plane0 rotate around the head, pull the faceTraker1 to the top before faceTraker0, just like the picture. To do that just click and drag faceTraker1 and drop it before faceTraker0. 



 Now we need to center the nullObject0 to the head. Select nullObject0, under faceTraker0, in The Scene plane, top left screen, change the Z Position properties to Z = -0.2, this is located in The Inspector, right side of screen.


Here is the before and after of how the head should look.

                           Before                                                        After


 We need to update plane0 to have it come in front and around the face. Select plane0 under faceTraker0 → nullObjects0 → plane0 in The Scene panel. In The Inspector, right side of screen, change the Position for Z to 0.2.
 

 Now lets set the newMateial to invisible by selecting newMaterial under The Assets panel → Materials → newMateral.


 In The Inspector, right side of screen, under Render Options → Opacity, set Opacity to 0 (zero).



### Step 6: Lets add our 3D object that will be floating around the head

 Under The Assets panel click on + Add Asset and select Search AR Library…









 In the pop-up click on 3D Shapes and select a shape. You can also import your own 3D object if you have one. 


 Get the 3D object and drag it under the nullObject0.





 Press the pause button on The Scene panel, top left menu on the screen. Select the 3D object. 


 In The Viewpoint use the blue arrow to pull the 3D object towards the checker box object. 




 Pull the green arrow up, pass the checker box object. Press play to see how your 3D item looks. Adjust and also resize as needed.



 If you are having a hard time seeing your image, you can change the color by selecting color under your object in the Assets Pane:

 Then select the color you want in the Inspector Pane

All Done. Your image should look something like this. 


Congratulations!  You have just created your very own AR filter.  Think of all the different possibilities you can do.  There are many other different templates built into Spark AR.  Give them a try and learn something new!  Don’t forget to have fun and share it with everyone!

