# CE597 --- 2021 Spring Class Demos
This is the class demos from CE 597 Machine Learning and Artificial Intelligence for Autonomous Vehicle Operations.



## Course outline

This class will include but not limited to the following topics (and their applications in transportation system and AV operations):

\-    Regression: Linear, 

\-    Classification: Perceptron, SVM, Logistic, Decision Tree.

\-    Model selection: Hyperparameter search, Cross-validation, Learning Curves, AIC, BIC.

\-    Classic data mining methods: Multi-Armed Bandits (MAB), Link Analysis and Prediction Heuristics (Link prediction, Missing values), Collaborative Filtering, Dimensionality Reduction.

\-    Improving Weak Models: Ensemble techniques, boosting

\-    Deep Learning: 

​	Artificial neural network

​	Feedforward Networks (activation functions, architectures, generalization, and universal approximators).

​	Backpropagation (chain rule of calculus, vanishing and exploding gradients).

\-    Reinforcement Learning:

​	Q learning (Q table method)

​	Deep Reinforcement Learning (DQN, Actor-Critic, etc.)



## Course materials fetch steps

- Download the material for the first time:

  Open the directory(folder) on your local machine

  - Windows user: Open your powershell at this folder

     by click file --> open windows powershell (better if use administrative powershell) 

  - Mac user: Open terminal at this 

  For the first time, you should clone the repository from git hub simply by the following command in powershell/ terminal

  ```
  git clone https://github.com/JiqianDong/CE597_2020s.git
  cd 20S_CE597
  ls
  ```

  ```cd``` command represent changing directory. ```ls``` is for showing the contents.

- For updating the materials

  Similar way open the terminal at the ```CE597_2020Fall``` folder 

  ```
  git pull
  ```

  If it doesn't work, try the following

  ```
  git add .
  git commit -m"my commit"
  git pull
  ```

```git add .``` command is for add your files in to your local memory,  the ``commit``  is for saving, then pull the updated files.

## Using Google Colab

- Establish a folder in your google drive (named as CE597)

- Open Colab and mount your own google drive

```
from google.colab import drive
drive.mount('/content/gdrive')
```

- Changing working directory to the newly built folder (CE597)
```
%cd /content/gdrive/MyDrive/CE597
```


## Simple git command

See the following [commands](https://dev.to/dhruv/essential-git-commands-every-developer-should-know-2fl)

## Simple Linux command

Linux commands are for your powershell/terminal

- Changing directory: ```cd``` 

  ```
  cd <folder_name>  ## move to the child folder inside your current folder
  cd c:/ ## only works on windows
  cd ..  ## To the parent folder
  ```

  Note:

   ``./`` : current directory

  ``../`` : parent directory

  ``/`` : For separation, only needed when you want to access the files in the directory 

- Show the files: ```ls```

  ```
  ls -l 
  ls 
  ```


- Open Jupiter notebook in powershell/terminal

  ```
  jupyter notebook
  ```

- Make directories

  ```
  mkdir <directory name>
  ```

