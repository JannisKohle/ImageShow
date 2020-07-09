# ImageShow

An app in which you can view images (and more)

## The problem:

Create an app in which you can move around images, like in a grid by pressing different keys.

## My solution:

I'll create a REST API using Express that will return some HTML, showing the
image. When you close the website, the next time you open it, it will redirect
to the last image displayed. I will do this by storing the image everytime you open it.
And when you just go to / , it will redirect to the correct page.

### The api:

In the rest api there are **2** endpoints:

- ```/```: This will redirect to the last image displayed
- ```/image?x=2&y=5```: This would show ```image_2_5.xyz```. On this page, when you press different keys, it will go to a different image.

## How to use it:

First, you need to changed the path to the folder containing all the images.
You can do that in the file ```imgPath.json```
In that folder, the images need to be called like a grid with x and y, e.g:

- ```image_1_1.xyz``` - ```image_1_2.xyz``` - ```image_1_3.xyz```

- ```image_2_1.xyz``` - ```image_2_2.xyz``` - ```image_2_3.xyz```

- ```image_3_1.xyz``` - ```image_3_2.xyz``` - ```image_3_3.xyz```
