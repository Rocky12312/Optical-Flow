# Optical-Flow

Optical flow is the pattern of apparent motion of image objects between two consecutive frames caused by the movement of object or camera. It is basically a 2D vector field where each vector is a displacement vector showing the movement of points from first frame to second.

Lucas Kanade algorithm:
The  Lucas-Kanade  optical  flow  algorithm  is  a  simple  technique  which  can provide  an  estimate  of  the  movement  of  interesting  features  in  successive images of a scene.  We would like to associate a movement vector (u,v) to every such interesting pixel in the scene, obtained by comparing the two consecutive images.The Lucas-Kanade algorithm makes some implicit assumptions:–  
The two images are separated by a small time increment ∆t, in such away that objects have not displaced significantly (that is,the algorithm works best with slow moving objects). 
The images depict a natural scene containing textured objects exhibiting shades of gray (different intensity levels) which change smoothly.The algorithm does not use color information in an explicit way.  It does not scan the second image looking  for a match for a given pixel.It works by trying to guess in which direction an object has moved so that local changesin intensity can be explained

Farneback method:
 Farneback algorithm to find the dense optical flow. It computes the optical flow for all the points in the frame. It is based on Gunner Farneback’s algorithm which is explained in Two-Frame Motion Estimation Based on Polynomial Expansion by Gunner Farneback in 2003.

The way to find the dense optical flow has been explained in the code.We get a 2-channel array with optical flow vectors, (u,v). We find their magnitude and direction. We can basically color code the result for better visualization. Direction will  corresponds to Hue value of the image.
