# CS230_Fall2021_Project by Umesh Thillaivasan

https://cs230.stanford.edu/project/

## Real world 3D object pose estimation and the Sim2Real gap (Vision)

Project Overview:
1. Reproduce PoseCNN https://rse-lab.cs.washington.edu/projects/posecnn/ and DOPE's https://docs.nvidia.com/isaac/isaac/packages/object_pose_estimation/doc/dope.html results to understand existing model architectures in this domain.
2. Create new 3D models of objects in CAD/blender, and set up a training dataset of {2D image, 3D pose} for each object
3. Use transfer learning and fine-tune the above models on these custom-made objects of interest
4. 3D print the objects and test their sim2real performance of the pose estimator
5. Finally, repeat steps 3 and 4, but now retrain the neural networks by using some domain randomization techniques (e.g., generating images of the custom objects with varying lighting textures etc); then re-evaluate how much that improves the performance on the real-world image dataset made in step 4.
