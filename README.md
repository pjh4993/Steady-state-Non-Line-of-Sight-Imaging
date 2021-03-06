# Steady-state-Non-Line-of-Sight-Imaging

This is the official code release for paper Steady-state Non-Line-of-Sight Imaging

## Usage

It contains 2 part, first is how to render data and second is how to train the neural network model.
 
### Render

We recommand to open it in Eclipse(tested), Nsight(tested) or Visual Studio. Other IDE should also work. To compile the code, please install libglm, glew, glfw and opencv.

```
sudo apt-get install libglm-dev
sudo apt-get install libglew-dev
sudo apt-get install libglfw3-dev
sudo apt-get install libopencv-dev
```

Next, put everything in render-mnist folder in the eclipse project and compile. To successfully run the code, modify the mnist folder path and data saving path in main.cpp (line85 and 90). Then click run button.

**Rendered image: orthogonal view image and steady state renderings with different light positions.**</br>
<img src="./renders/original-0-0.4703.png" width = "200px" />
<img src="./renders/combine-light_0_5.png" width = "200px" />
<img src="./renders/combine-light_3_0.png" width = "200px" />
<img src="./renders/combine-light_6_2.png" width = "200px" />


### Deep Learning Model

We use tensorflow 1.10. Note that tensorflow 2.0 is not tested!

To run the code, modify the config.py in dl-mnist folder, change the datafolder term to the rendered data folder. Then run
```
python train.py
```

### Captured Data

We capture 10 examples, including 3 mnist examples and 7 shapenet examples. We will upload soon.

**Captured Data: side view image, our reconstruction and captures**</br>
<img src="./captures/Screenshot from 2020-01-28 22-45-08.png" width = "200px" />
<img src="./captures/Screenshot from 2020-01-28 22-45-14.png" width = "200px" />
<img src="./captures/input_5.png" width = "200px" />
<img src="./captures/input_2.png" width = "200px" />



### citation
If you find it is useful, please cite


  @InProceedings{chen_2019_nlos,
  
     author={Chen, Wenzheng and Daneau, Simon and Mannan, Fahim and Heide, Felix},
  
     title={Steady-state Non-Line-of-Sight Imaging},
     
     booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
     
     month = {June},
     
     year = {2019}
  
  }
