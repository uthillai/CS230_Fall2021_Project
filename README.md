# CS230_Fall2021_Project by Umesh Thillaivasan

https://cs230.stanford.edu/project/

## Real world 3D object pose estimation and the Sim2Real gap (Vision)

### Project Overview:
1. Reproduce DOPE https://docs.nvidia.com/isaac/isaac/packages/object_pose_estimation/doc/dope.html results to understand existing state-of-the-art model architectures in this domain
2. Create new 3D models of objects in CAD & Unreal Engine 4 using NVIDIA's Deep Leaning Dataset Synthesizer plug-in, and set up a training dataset of {2D image, 3D pose} for a custom class generating synthetic data using domain randomization (e.g., generating images of the custom objects with varying lighting textures etc)
3. Use transfer learning and fine-tune the above models on these custom-made objects of interest
4. 3D print the objects and test their sim2real performance of the pose estimator
5. Perform sensitivity analysis on synthetic data to explore which variables impact performance and how that fits real-world experience

Examples of 3D CAD models that are 3D printed, then a real-world image with an initial synthetic image, both with a wood grain background.
![tetris_CAD](https://user-images.githubusercontent.com/25275773/144511365-9839fe00-d8fd-446a-aad9-be4c43882f83.png)
![tetris_slicer](https://user-images.githubusercontent.com/25275773/144511361-a85a3885-9ec0-4e52-a058-35d37b0138f6.png)
![3Dprinttestsetup](https://user-images.githubusercontent.com/25275773/144511366-9959d6e4-0f9f-449d-be36-1a9f9e8bdce3.JPG)
![IMG_4636](https://user-images.githubusercontent.com/25275773/144511413-5a0d34cf-df50-49b9-b31f-a7efe8efd0c6.jpg)


## How to run testing with DOPE.
1. modify my_config_webcam.yaml file to include custom class and weights path
2. update live_dope_webcam.py with img paths to test images

## Examples of synthetic data generated
![000003 right-2](https://user-images.githubusercontent.com/25275773/144511304-b8c0294d-420a-4f56-b338-0522bb86bdb6.png)
![000003 left](https://user-images.githubusercontent.com/25275773/144511306-535741fa-3389-40cc-858d-98ac49e1e997.png)
![000001 right-2](https://user-images.githubusercontent.com/25275773/144511308-294e8142-3ab1-4564-bec1-ef0f59e7fd28.png)
![000010 left](https://user-images.githubusercontent.com/25275773/144511310-ed566569-3fcd-477d-9ad3-3532a9937aba.png)
![000003 right](https://user-images.githubusercontent.com/25275773/144511311-bfc529cf-e197-4b18-af43-ed55627436ed.png)
![000004 left-2](https://user-images.githubusercontent.com/25275773/144511313-00b6ceee-493d-421e-99ed-a84064c1f30f.png)
