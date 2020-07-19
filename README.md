# Cartoonize Your Image!

**The web app for this image cartoonization: https://image-cartooning-app.herokuapp.com/**

This is a web app to turn your photo into a cartoon-like image. There are four filters that you can choose from: Pencil Sketch, Detail Enhancement, Pencil Edges, and Bilateral Filter. Below is the example of the cartoonization after you apply each filter:

**Pencil Sketch:**

<p align="center">
  <img width="700" height="350" src=https://github.com/marcellusruben/Image_Cartooning_Web_App/blob/master/image/pencil_sketch.png>
</p>

**Detail Enhancement:**

<p align="center">
  <img width="700" height="350" src=https://github.com/marcellusruben/Image_Cartooning_Web_App/blob/master/image/detail_enhancement.png>
</p>

**Pencil Edges:**

<p align="center">
  <img width="700" height="350" src=https://github.com/marcellusruben/Image_Cartooning_Web_App/blob/master/image/pencil_edges.png>
</p>

**Bilateral Filter:**

<p align="center">
  <img width="700" height="350" src=https://github.com/marcellusruben/Image_Cartooning_Web_App/blob/master/image/bilateral_filtering.png>
</p>

## Files

There are five files necessary to build this web app:

- cartoon_app.py: main Python file of the app.
- setup.sh: file to setup your configuration on Heroku.
- requirements.txt: the file to tell Heroku which dependencies you need to build the app.
- Procfile: file to tell Heroku which and how the command and file should be executed.
- Aptfile: additional file for buildpacks to enable OpenCV to operate within Heroku.

In your Heroku app that you can access on Heroku, you need to add this buildpack: https://github.com/heroku/heroku-buildpack-apt to complement the Aptfile.

To add the buildpack: Go to your app on Heroku -> choose "Setting" tab on your app -> Then scroll down until you find Buildpacks section -> Click on "add buildpacks" -> paste the above URL.

With Heroku CLI you can use this command to add the buildpacks: 

```
heroku create --buildpack https://github.com/heroku/heroku-buildpack-apt.git
```


