# CS230_Fall2021_Project by Umesh Thillaivasan

https://cs230.stanford.edu/project/

## Real world 3D object pose estimation and the Sim2Real gap (Vision)

Project Overview:
1. Reproduce PoseCNN https://rse-lab.cs.washington.edu/projects/posecnn/ and DOPE's https://docs.nvidia.com/isaac/isaac/packages/object_pose_estimation/doc/dope.html results to understand existing model architectures in this domain.
2. Create new 3D models of objects in CAD/blender, and set up a training dataset of {2D image, 3D pose} for each object
3. Use transfer learning and fine-tune the above models on these custom-made objects of interest
4. 3D print the objects and test their sim2real performance of the pose estimator
5. Finally, repeat steps 3 and 4, but now retrain the neural networks by using some domain randomization techniques (e.g., generating images of the custom objects with varying lighting textures etc); then re-evaluate how much that improves the performance on the real-world image dataset made in step 4.

Examples of 3D CAD models that are 3D printed, then a real-world image with an initial synthetic image, both with a wood grain background.
![WhatsApp Image 2021-11-05 at 12 49 27 PM](https://user-images.githubusercontent.com/25275773/140565258-fcda7c61-a207-4999-92c2-c8534bc3b5c2.jpeg)
![WhatsApp Image 2021-11-05 at 12 49 10 PM](https://user-images.githubusercontent.com/25275773/140565259-4137c5af-527b-4310-8b27-5930b9be5c1d.jpeg)
![WhatsApp Image 2021-11-05 at 9 31 54 AM](https://user-images.githubusercontent.com/25275773/140565262-f9f7be90-49d0-411c-a9e8-03dc999ccd5a.jpeg)


## How to run testing with DOPE.
1. modify my_config_webcam.yaml file to include custom class and weights path
2. update live_dope_webcam.py with img paths to test images
