# City1M-dataset
First synthetic group re-identification dataset with over 100,000,000 images (CVPR2022).

## Overview
The proposed City1M is constructed by collecting images from 8 street cameras in a city scene, which contains 1.84M RGB images with a uniform resolution of 1920 x1080, 45,000 persons and 11,000 groups. Our dataset also includes day and night scenes.

![78f6183fcfc5f6eb17f10970accd0dd](https://user-images.githubusercontent.com/16618172/159493302-7159031b-429b-46a6-8dca-dbc32c802cff.png)




## Dataset format

We provide a full version of the City1M (named **City1M-full**), a simplified version (named **City1M-lite**), and related person models (named **City1M-personModels**).

### City1M-full
The City1M-full consists of 6 zip files, named Images_x.zip, x=2,3,4,5,6. For example, the format of image name in each zip file is:
> Images_2/0009501_pCount2_cam1_0000001_day.jpg


* '00095001' is the group id of this image.
* 'pCount2' is the number of member. (this only used for creating datraset, maybe not useful for you.)
* 'cam1' is the camera id.
* '00000001' is the index. (it also make no sense for you.)
* 'day' is a coarse time label (totally two labels, 'day' or 'night').

We provide two protocols as follows:
* Procotol@1 = train_part1.txt + query_part1.txt + gallery_part1.txt
* Procotol@2 = train_part2.txt + query_part2.txt + gallery_part2.txt

Each line in txt file is a label of the image:
> 0009501_pCount2_cam1_0000001_day.jpg 0,1477.3156,230.6843,186.0616,346.3864,1.5166 1,1752.9762,215.4119,153.7662,221.532,2.6906

Each line is split by ' ', the first item is the image name, and the following items are the annotations for each member, for example:
> 0,1477.3156,230.6843,186.0616,346.3864,1.5166

* 0 is the person id of the first member.
* 1477.3156,230.6843,186.0616,346.3864 is the (x,y,h,w) of the first member.
* 1.5166 is depth between the camera and the first member.

### City1M-lite


### City1M-personmodel

## Dataset Applcation
If you are interested in our dataset, please feel free to fill in the application form (PDF) and send it to email zhangq48@mail2.sysu.edu.cn, and we will reply to you as soon as possible.


