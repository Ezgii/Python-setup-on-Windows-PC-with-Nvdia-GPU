
1. [Download](https://www.anaconda.com/) and install Anaconda for Windows.
   
   Verify that conda is installed:
   
   ![image](https://github.com/Ezgii/GPU/assets/4748948/e9f7d2df-a7d2-4352-b93a-929116a426c6)

4. Create an environment:
   
   `conda create -n <env_name>`
   
   `conda activate <env_name>`
   
   `conda install -c anaconda ipykernel`

   `python -m ipykernel install --user --name=<env_name>`

   `conda install numpy`

   `conda install matplotlib`
   
   `conda install pytorch torchvision torchaudio pytorch-cuda=11.6 -c pytorch -c nvidia`

      - Note: To determine which Pytorch version to install, go to https://pytorch.org/ and select the appropriate configuration, as shown below.
  
        ![image](https://github.com/Ezgii/GPU/assets/4748948/54fafee5-7f3f-4bc8-bd01-babd070ceed0)
      
        To learn which CUDA version you have, run `nvcc --version` command. The `nvdia-smi` command shows the highest CUDA version the installed driver supports on the top right corner of the command's output. Note that this does not mean that CUDA version is installed. It may or may not be. You can check via `nvcc --version` command if CUDA is really installed. My CUDA version is 11.6.
   
        
        ![image](https://github.com/Ezgii/GPU/assets/4748948/eb92cec3-9ae4-4b75-bf78-4affacfeba3c)

     

   
