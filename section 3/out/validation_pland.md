### What is the intended use of the product?
 As identifying the volume of the hippocampus using MRI scans is quite since every slice of 3D volume needs to be analyzed. So, using this system we can quantify disease progression over time for the patients which are showing early symptoms of Alzheimer's disease.
 SO this algorithm/system can help clinicians perform this taks quite faseter and consitently as this this sytem can automatically measure hippocampal volumes with posterior and anterior of new patients.


### How was the training data collected?
The "Hippocampus" dataset from the [Medical Decathlon competition](http://medicaldecathlon.com/index.html).
This dataset is stored as a collection of NIFTI files, with one file per volume, and one file per corresponding segmentation mask.
The original images here are T2 MRI scans of the full brain. 
In this dataset, volumes have been cropped where only the region around the hippocampus has been cut out.
This makes the size of our dataset quite a bit smaller.

### How did you label your training data?

All data has been labeled and verified by an expert human rater.
The whole dataset will be made available online to be shared and improve upon under the copyright license (CC-BY-SA 4.0).


### How was the training performance of the algorithm measured and how is the real-world performance going to be estimated?
Our algorithm processes consistent similar to what has been used during training. For the performance measuserment, we are using Jaccard and Dice similarity metrics. It uses the Jaccard distance from the labels to compute the Dice and jaccard similarity which assess how close our volumes are to each other.

In the real world, doctors or imaging department can put a certain tag into the series description and then our system would process those series only that have that particular tag. And tag that will be used can be decided between our algorithm and imaging department or doctor.

### What data will the algorithm perform well in the real world and what data it might not perform well on?

The system will perform best in the real if the data presents a clear view of hippocampus and patient should not have any other disease which may affect the algorithm's performance.
