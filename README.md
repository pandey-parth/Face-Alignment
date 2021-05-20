# Face-Alignment
In this task, you have to implement face normalization and alignment. Most of the face images deceptively seem to be aligned, but since many face recognition algorithms are very sensitive to shifts and rotations, we need not only to find a face on the image but also normalize it. Besides, the neural networks usually used for recognition have fixed input size, so, the normalized face images should be resized as well.

There are six images of faces you have to normalize. In addition, you have the coordinates of the eyes in each of the pictures. You have to rotate the image so that the eyes are on the same height, crop the square box containing the face and transform it to the size 224×224.

The eyes should be located symmetrically and in the middle of the image (on the height).

You get the images and corresponding eyes coordinates for each person. You should implement the function 𝚕𝚘𝚊𝚍 _𝚏𝚊𝚌𝚎𝚜_𝚊𝚗𝚍_𝚎𝚢𝚎𝚜 that reads the data and returns two dictionaries: the dictionary of images and the dictionary of eyes coordinates. Eyes coordinates is a list of two tuples [(𝑥1,𝑦1),(𝑥2,𝑦2)]

. Both dictionaries should have filenames as the keys.

𝚍𝚒𝚛 _𝚗𝚊𝚖𝚎 is the path to the directory with face images, 𝚎𝚢𝚎_𝚙𝚊𝚝𝚑 is the path to `eyes.pickle` file with eyes coordinates. If these directory and file are located in the same directory as this notebook, then default arguments can be used.

Some Face images-

![](https://github.com/pandey-parth/Face-Alignment/blob/master/faces_imgs/1.jpg) ![](https://github.com/pandey-parth/Face-Alignment/blob/master/faces_imgs/5.jpg)

**Converted to**

![](https://github.com/pandey-parth/Face-Alignment/blob/master/Screenshot/Screenshot_2021-05-20%20face_alignment%20-%20Jupyter%20Notebook(1).png) ![](https://github.com/pandey-parth/Face-Alignment/blob/master/Screenshot/Screenshot_2021-05-20%20face_alignment%20-%20Jupyter%20Notebook.png)
