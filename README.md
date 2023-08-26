# GPU

1. Download Anaconda for Windows:
   https://www.anaconda.com/

2. How to install Pytorch:

   - Go to https://pytorch.org/ and select the appropriate configuration, as shown below. To learn which CUDA version you have, run `nvcc --version` command. The `nvdia-smi` command shows the highest CUDA version the installed driver supports on the top right corner of the command's output. Note that this does not mean that CUDA version is installed. It may or may not be. You can check via `nvcc --version` command if CUDA is really installed.
     ![image](https://github.com/Ezgii/GPU/assets/4748948/eb92cec3-9ae4-4b75-bf78-4affacfeba3c)


      Copy the command and run it on the command prompt.
     (I run `conda install pytorch torchvision torchaudio pytorch-cuda=11.6 -c pytorch -c nvidia` because my CUDA version was 11.6.)
     ![image](https://github.com/Ezgii/GPU/assets/4748948/54fafee5-7f3f-4bc8-bd01-babd070ceed0)

3. Create an environment:
   
   `conda create -n thesis`
   
   `conda activate thesis`
   
   `conda install ipykernel`
