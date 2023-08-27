
1. [Download](https://www.anaconda.com/) and install Anaconda for Windows.
   
   Verify that conda is installed:
   
   ![image](https://github.com/Ezgii/Python-setup-on-Windows-PC-with-Nvdia-GPU/assets/4748948/a1fa5fc1-b84a-466b-b7d4-a433055fdd6d)

2. Create an environment and install the dependencies:
   
   `conda create -n <env_name>`
   
   `conda activate <env_name>`
   
   `conda install -c anaconda ipykernel`

   `python -m ipykernel install --user --name=<env_name>`

   `conda install numpy`

   `conda install matplotlib`

   To install Pytorch using conda:
   
   `conda install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia`

   To install Pytorch using pip:

   `C:\Users\Ezgi>pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117`

      - Note: To determine which Pytorch version to install, go to https://pytorch.org/ and select the appropriate configuration, as shown below.
  
        ![image](https://github.com/Ezgii/Python-setup-on-Windows-PC-with-Nvdia-GPU/assets/4748948/70559d1d-b0e6-4203-9340-7e6b6d72922e)

        To learn which CUDA version you have, run `nvcc --version` command. The `nvdia-smi` command shows the highest CUDA version the installed driver supports on the top right corner of the command's output. Note that this does not mean that CUDA version is installed. It may or may not be. You can check via `nvcc --version` command if CUDA is really installed. My CUDA version is 11.6.
   
        
        ![image](https://github.com/Ezgii/Python-setup-on-Windows-PC-with-Nvdia-GPU/assets/4748948/5ac5610c-62a5-46ce-9e5b-7eb6b88cb697)


3. Open Jupyter notebook. Select <my_env> as the kernel. Verify that torch is installed with CUDA support, as below:

![image](https://github.com/Ezgii/Python-setup-on-Windows-PC-with-Nvdia-GPU/assets/4748948/f18e3c3f-5016-4fd4-a45f-8de9378a3a20)



     

   
