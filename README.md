# ■mnister
You can easily make AI recognize the numbers you wrote.
The execution environment of mnister can be executed on Google Colab or Local PC.
  
## ☁：When running on Google Colab
see -> https://github.com/PoodleMaster/mnister/blob/master/mnister.ipynb

### 1. Requirements
- flask_ngrok 

### 2. Build Python Environment
Load **'mnister.ipynb'** in Google Colab and execute all cells.

### 3. Install mnister:
```ipynb
!git clone https://github.com/PoodleMaster/mnister.git
```

### 4. Install python libraries:
```ipynb
%cd mnister
!pip install flask_ngrok
```

### 5. Usage
Start the server and client.

#### (1) Server startup
```ipynb
!python server.py --colab
```

#### (2) Client startup 
Start your browser and access the following URL:(http://xxxxxxxxxxxx.ngrok.io)

### 6. Execution Sample
![mnister sample ngrok](https://user-images.githubusercontent.com/69660581/93540466-b4ab0300-f98e-11ea-843b-6399cdbce4c2.gif)

## 💻：When running on Local PC

### 1. Requirements
- Anaconda : 3
- Python : 3.7
- Tensorflow : 2.3.0 (Please use the same version as when you created the model.)
- flask pillow matplotlib
- flask_ngrok 

### 2. Build Python Environment
```cmd
c:\>conda create -n mnister37 python=3.7
c:\>conda activate mnister37
```

### 3. Install mnister
```cmd
(mnister37) c:\>git clone https://github.com/PoodleMaster/mnister.git
```

### 4. Install python libraries:
```cmd
(mnister37) c:\>cd mnister
(mnister37) c:\mnister>conda install flask pillow matplotlib
(mnister37) c:\mnister>pip install tensorflow==2.3.0
(mnister37) c:\mnister>pip install flask_ngrok
```
- Use the same version of Tensorflow as when you created the model.
- The Tensorflow version of the included model is 2.3.0.

### 5. Usage
Start the server and client.

#### (1) Server startup
```cmd
(mnister37) c:\mnister>python server.py
```
#### (2) Client startup 
Start your browser and access the following URL:(http://127.0.0.1:5000)

### 6. Execution Sample
![mnister sample localhost](https://user-images.githubusercontent.com/69660581/93540433-9d6c1580-f98e-11ea-97e0-ec2d3b98326a.gif)

# ■Create MNIST model
If you want to create a MNIST model, please use **'CreateMnistModel.ipynb'**.

## ☁：Running on Google Colab
see -> https://github.com/PoodleMaster/mnister/blob/master/CreateMnistModel.ipynb

### 1. Build Python Environment
Load **'CreateMnistModel.ipynb'** in Google Colab and execute all cells.

### 2. Create MNIST model
1. Set [Runtime]-[Change Runtime Type]-[Hardware Accelerator] to GPU
2. Execute [Runtime]-[Execute all cells]
3. Make sure you have an hdf5 file at the following:(GoogleColab:/content/colab_mnist.hdf5)
4. Make sure the hdf5 file is downloaded.<BR>

![model download](https://user-images.githubusercontent.com/69660581/93541052-639c0e80-f990-11ea-8d13-e695278f3611.png)

### 3. Set Your Created MNIST model
Replace it with the hdf5 file stored directly under mnister(mnister/colab_mnist.hdf5). 
- When running on Google Colab<BR>

![Replace](https://user-images.githubusercontent.com/69660581/93542177-4ae12800-f993-11ea-9c00-3449b00b2d31.png)

- When running on Loacl PC<BR>

![Replace](https://user-images.githubusercontent.com/69660581/93542613-71ec2980-f994-11ea-95a6-46e82c0e3229.PNG)

# ■Contributing
Contributions, issues and feature requests are welcome.

# ■Author
- Github: [PoodleMaster](https://github.com/PoodleMaster)

# ■License
Check the LICENSE file.
