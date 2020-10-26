# How To Make Your Own Quarantine Wedding AR Filter

## Introduction:
In this tutorial, you will be learning how to use Spark AR to create your own AR Filter using Head Occluder and 3D Objects.   Covid-19 has changed the way we interact as a community.  With this AR filter, you can allow people to be part of the event without actually being there.  Your friends and family that can’t make it can utilize this filter and share on their Instagram. 
 
## You will learn:
1.  Downloading and setting up Spark AR Studio
2.  Creating and modifying a head tracking project
3.  Adding objects and animations
4.  Utilizing the Head Occluder
5.  Putting all together to make the filter

This tutorial is for complete beginners and just assumes you have access to a computer that can run Spark AR.  Not required, but nice to have would be pre existing digital objects that you want to incorporate into your filter.  

## Getting Started:

In order for this to work best, you can create your own 3D object.  This tutorial assumes you already have a 3D object or that you will be using one of the built in assets available in Spark AR Studio.  If you want to create your own 3D asset, you can do so in either Tinkercad.com or by using Paint 3D in Windows 10.  This entire tutorial can be done using default assets, but for the best effect, you’ll want to bring in your own 3D objects.  

### Step 1: Download Spark AR Studio

1. Go to https://sparkar.facebook.com/ar-studio
2. Click on **Download** on the top right corner, pink button.
![image](https://user-images.githubusercontent.com/466483/97206191-a0b8a500-1775-11eb-9013-2ee2498610af.png)
3. Then click on the next pink button that says **Download**. 
![image](https://user-images.githubusercontent.com/466483/97207127-e0cc5780-1776-11eb-998e-437354aed499.png)

And that’s it.  Depending on your internet connection, it will take a few minutes to download.  Now, let’s install the software!

### Step 2: Installing Spark AR Studio

1. Click on the downloaded image called **SparkARStudio_v98.msi**.

2. Follow the instructions to install. Click on **Next**.<br />
![image](https://user-images.githubusercontent.com/466483/97206821-7c10fd00-1776-11eb-8b9f-aa00b2015be0.png)

3. Read and accept terms in the License Agreement. Click on **Next**. <br />
![image](https://user-images.githubusercontent.com/466483/97206960-a498f700-1776-11eb-9a5a-658d671dce72.png)

4. Follow special instructions for iOS users. Click **Next**. <br />
![image](https://user-images.githubusercontent.com/466483/97206992-b2e71300-1776-11eb-9fa0-5b76cca98b01.png)

5. This screen is just to keep older versions of Spark AR Studio on your computer. Check the box if that is what you want to do. Then click on **Next**. <br />
![image](https://user-images.githubusercontent.com/466483/97207038-c1352f00-1776-11eb-8519-d3ce88d8f4df.png)

6. Choose where you want the program to be installed. Click on **Next**. <br />
![image](https://user-images.githubusercontent.com/466483/97207179-f17ccd80-1776-11eb-9e77-cbdbd877ccfe.png)

7. Finally, click on **Install**. Note: you might get a pop-up window that says that this installation will change some devices. Click on **Yes**, then it will finish installing. <br />
![image](https://user-images.githubusercontent.com/466483/97207244-06596100-1777-11eb-9d71-18f8e726c84d.png)

Now that you have the software installed, it’s time to roll up your sleeves and start creating.  This tool is super powerful and there’s a lot going on.  


### Step 3: Starting your first project

1. Open Spark AR Studio and log in.
2. Click on **New Project**. <br /> 
![image](https://user-images.githubusercontent.com/466483/97208072-f5f5b600-1777-11eb-9881-153d6dac5d28.png)

3. On the pop-up screen select **Blank Project**. <br />
![image](https://user-images.githubusercontent.com/466483/97208195-19b8fc00-1778-11eb-89a6-534203828f41.png)

4. Click on **+ Add Object**, located in the *The Scene panel*, top left section of screen. <br />
![image](https://user-images.githubusercontent.com/466483/97208367-4a009a80-1778-11eb-8681-c60a529d00f4.png)

5. On the pop-up select **Face Tracker** and then click on the **Insert** button. <br />
![image](https://user-images.githubusercontent.com/466483/97208443-5f75c480-1778-11eb-96bb-cd20fb980fcf.png)

6. Right click on **faceTraker0**, located in *The Scene panel*, top left section, go to **Add → Null Object**. <br />
![image](https://user-images.githubusercontent.com/466483/97208584-88965500-1778-11eb-80d5-f5625121a32a.png)

This will add the item below to **The Viewport**. <br />
![image](https://user-images.githubusercontent.com/466483/97208645-951aad80-1778-11eb-9452-34e26bc0ecae.png)

7. Right click on **faceTraker0**, located in *The Scene panel*, top left section, go to **Add → Plane**. <br />
![image](https://user-images.githubusercontent.com/466483/97208743-b4b1d600-1778-11eb-9716-e8a836afaf11.png)

This will add the checker box to The Viewport. <br />
![image](https://user-images.githubusercontent.com/466483/97208778-be3b3e00-1778-11eb-85fa-4bd22df49094.png)

8.Drag plane0, located in The Scene panel, into nullObject0. It should look like this. <br />
![image](https://user-images.githubusercontent.com/466483/97208837-cf844a80-1778-11eb-895a-f710a704b161.png)

9. On the top menu, click on **View → Show/Hide Patch Editor** <br />
![image](https://user-images.githubusercontent.com/466483/97208900-e5920b00-1778-11eb-9bdf-86babf68f91f.png)


### Step 4: Adding the Animation Loop

1. With **plane0** selected, right click in the **Patch Editor**, select **Animation --> Loop Animation** and then click on the button **Add Patch**. <br />
![image](https://user-images.githubusercontent.com/466483/97209326-6b15bb00-1779-11eb-8cef-25da9b7d391a.png)

A **Loop Animation** block should show in the **Patch Editor**. <br />
![image](https://user-images.githubusercontent.com/466483/97209380-8254a880-1779-11eb-96b0-137defef309c.png)

2. With **plane0** selected, right click in the **Patch Editor**, select **Animation → Transitions** then click on the button **Add Patch**. <br />
![image](https://user-images.githubusercontent.com/466483/97209497-a6b08500-1779-11eb-9cfb-2ec7ec5367f0.png)

A **Transition** block should show in the **Patch Editor**. <br />
![image](https://user-images.githubusercontent.com/466483/97209616-cc3d8e80-1779-11eb-91b3-18938d34b6b0.png)

3. Select the nullObject0, located in The Scene panel, top left side of screen. In the The Inspector on the right side of the screen, click on the arrow in front of Rotation. This will turn the Rotation section yellow as shown below and a yellow block will appear in the Patch Editor. Link the Transition block to the Rotation block by clicking on the arrow located at the end of the Transition block and connecting it to the arrow in front of the Rotation block.  <br />
![image](https://user-images.githubusercontent.com/466483/97210332-ae245e00-177a-11eb-9412-cd0920049244.png)
4. In the Transition block change the End values to x = 0, y = 360, and z = 0. This change will make the checker box speed in front of the person’s face. <br />
![image](https://user-images.githubusercontent.com/466483/97210365-b9778980-177a-11eb-9064-c22050ee4443.png)

5. In the Loop Animation block change Duration to 5. This change will make the checker box spin slower. <br />
![image](https://user-images.githubusercontent.com/466483/97210397-c3998800-177a-11eb-9517-8a0949846957.png)

6. Select plane0, located in The Scene panel, top left side of screen. Then set  Z = 0.1 for the Position, located in The Inspector,  on the right side of the screen. This change will make the checker box spin and go around in front of the person’s face. Make the plane0 invisible by unchecking Visible on the Properties menu on The Inspector, right side of the screen. This will make the checker box disappear. <br />
![image](https://user-images.githubusercontent.com/466483/97210467-d6ac5800-177a-11eb-89c7-9aff145243ec.png) <br />
![image](https://user-images.githubusercontent.com/466483/97210505-e461dd80-177a-11eb-94f0-55d7229a2911.png)

### Step 5: Working with Head Occluder 

1. Now we need the Head Occluder. To get the Head Occluder go download the Head Occluder from https://sparkar.facebook.com/ar-studio/learn/articles/people-tracking/face-reference-assets#whats-included-in-the-face-reference-assets 

2. Click on Download the Face Reference Assets here.

3. A zip folder will be downloaded to your computer. Unzip the folder wherever you would like to save the content of the zip folder. In the The Assets panel, bottom left of screen,  click From Computer. Browse to the location where you unzip your download. Open headOccluder.obj. In my case I saved mine to my documents at C:\User\Documents\FaceAssets\Mesh\headOccluder.obj

The Assets panel, should look like this. 

4. Add another Face Tracker to The Scene panel, top left of screen, you should have two face trackers now. Click on + Add Object → Face Tracker → Insert. 



5. Right click on faceTraker1, then Add → Face Mesh.


You should now see a checker pattern on the face of the person. Like this. 


6. Drag the headOccluder object in The Assets panel, bottom left section, to the faceTraker1 object, in The Scene panel, top left section. 


This is what you will see in The Viewport. 


7. With the headOccluder selected go to the The Inspector, located on the right side of screen, change Scale to X = 0.19, Y = 0.19, Z = 0.19. Play around with those values they may vary from screen to screen. It has to be larger than the human head, but not too big. 


8. Delete from The Assets panel, bottom left of screen, DefaultMaterial. Right click on DefaultMaterial then select Delete.

9. In The Assets pane, located at the bottom left of screen, add an asset by clicking on + Add Asset and click on Material. You may rename it if you want, for the purpose of this tutorial this material will be named newMaterial. 


10. With newMaterial selected in the The Assets panel, go to The Inspector, right side of screen and change Shader Type to Flat. 


The figures should look like this. 



11. Select faceMesh0 under faceTracker1 on the The Scene panel, then in The Inspector, right side of screen, add newMaterial to Materials by clicking the plus sign and selecting newMaterail. 





12. Select defaultobject under headOccluder in The Scene panel, top left side of screen. In The Inspector, the right side of the screen, change Material property to newMaterial. 


13. In The Assets panel, bottom left of screen, select newMaterial. In The Inspector, the rightside of the screen, change the Opacity to 30 to be able to see the person's face. This will change later to 0 (zero).


14. Select plane0 under faceTracker0 → nullObject0 → plane0 in The Scene panel, top left side of screen. In The Inspector, on the right side of the screen, check the Visible box to make the plane0 visible. 
 

The image of the person should look like this. 


15. To make the plane0 rotate around the head, pull the faceTraker1 to the top before faceTraker0, just like the picture. To do that just click and drag faceTraker1 and drop it before faceTraker0. 

16. Now we need to center the nullObject0 to the head. Select nullObject0, under faceTraker0, in The Scene plane, top left screen, change the Z Position properties to Z = -0.2, this is located in The Inspector, right side of screen.


Here is the before and after of how the head should look.

                           Before                                                        After


17. We need to update plane0 to have it come in front and around the face. Select plane0 under faceTraker0 → nullObjects0 → plane0 in The Scene panel. In The Inspector, right side of screen, change the Position for Z to 0.2.
 

18. Now lets set the newMateial to invisible by selecting newMaterial under The Assets panel → Materials → newMateral.


19. In The Inspector, right side of screen, under Render Options → Opacity, set Opacity to 0 (zero).



### Step 6: Lets add our 3D object that will be floating around the head

1. Under The Assets panel click on + Add Asset and select Search AR Library… <br />
![image](https://user-images.githubusercontent.com/466483/97211554-70c0d000-177c-11eb-814a-7a9c0f4d0931.png)

2. In the pop-up click on 3D Shapes and select a shape. You can also import your own 3D object if you have one. <br />
![image](https://user-images.githubusercontent.com/466483/97211502-61da1d80-177c-11eb-9b64-58530929eb32.png)

3. Get the 3D object and drag it under the nullObject0. <br />
![image](https://user-images.githubusercontent.com/466483/97211462-51c23e00-177c-11eb-9bb1-a86ffb7f38d4.png)

4. Press the pause button on The Scene panel, top left menu on the screen. Select the 3D object. <br />
![image](https://user-images.githubusercontent.com/466483/97211434-48d16c80-177c-11eb-907d-2175ac90d2c6.png)

5. In The Viewpoint use the blue arrow to pull the 3D object towards the checker box object. <br />
![image](https://user-images.githubusercontent.com/466483/97211405-3e16d780-177c-11eb-87b1-d623bd1fd5af.png)

6. Pull the green arrow up, pass the checker box object. Press play to see how your 3D item looks. Adjust and also resize as needed. <br />
![image](https://user-images.githubusercontent.com/466483/97211368-30615200-177c-11eb-84ca-90fbcce98b8b.png)

7. If you are having a hard time seeing your image, you can change the color by selecting color under your object in the Assets Pane: <br />
![image](https://user-images.githubusercontent.com/466483/97211266-060f9480-177c-11eb-8104-33bb498d7cfb.png)

8. Then select the color you want in the Inspector Pane <br />
![image](https://user-images.githubusercontent.com/466483/97211043-b16c1980-177b-11eb-9075-e32d97fc0bc2.png)

All Done. Your image should look something like this. <br />
![image](https://user-images.githubusercontent.com/466483/97211000-a31dfd80-177b-11eb-8400-0d54abbe49c4.png)

Congratulations!  You have just created your very own AR filter.  Think of all the different possibilities you can do.  There are many other different templates built into Spark AR.  Give them a try and learn something new!  Don’t forget to have fun and share it with everyone!

