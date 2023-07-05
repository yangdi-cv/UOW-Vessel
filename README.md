# UOW-Vessel: A Benchmark Dataset of High-Resolution Optical Satellite Images for Vessel Detection and Segmentation

## Dataset Overview
In this paper, we introduce UOW-Vessel, a new benchmark dataset of high-resolution optical satellite images for vessel detection and segmentation. Our dataset consists of 3,500 images, collected from 14 countries across 4 continents. With a total of 35,598 instances in 10 vessel categories, UOW-Vessel is the largest satellite image dataset for vessel recognition. Furthermore, compared to the existing public datasets that only provide bounding box ground-truth, our new dataset offers more accurate polygon annotations of vessel objects. Our dataset is expected to support segmentation-based approaches, which is a less investigated area in vessel surveillance.

## Dataset Examples
 <img src="https://github.com/ltb801/UOW-Vessel/blob/main/image/visualization.jpg?raw=true" height="270"/>

## Dataset Statistics
The UOW-Vessel dataset consists of 3,500 total images with the image resolution ranging from 8192 x 4320 to 8192 x 6881 pixels. The dataset is partitioned into the training, validation and test sets with the proportions of 70%, 10% and 20%, respectively. 

**Category statistics** There are 10 vessel categories present in our dataset. Table \ref{tbl:dataset_stats} shows the distribution of the number of instances per category in each set. The distribution indicates that there is an inherent class imbalance in the dataset, as 68.6\% of the instances belong to the Civilian category. The class imbalance reflects the real life scenarios, where civilian vessels tend to outnumber other classes, and certain classes like aircraft carriers and cruisers have fewer instances. Additionally, Figure \ref{fig:class_per_image} presents the distribution of the unique class counts per image. Overall, 55.11\% of the dataset has 1 unique class present in an image. The largest number of unique classes an image has is 7 classes, and these images account for only 0.37\% of the dataset. 

**Instance statistics** Our dataset consists of 35,598 instances in total. On average, each image is annotated with 10.2 instances. The most instances an image has in our dataset is 682 of mostly civilian vessel objects. Figure \ref{fig:instance_per_image} shows the distribution of the number of vessel instances per image. Furthermore, most of the vessel instances in our dataset have a relatively small size compared to the image size. Figure \ref{fig:mask_size} illustrates the relative size distribution of the instance masks. The distribution shows that approximately 65.4\% of the instances have a relative area smaller than 5\% of the image area. 
