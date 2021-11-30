## torch-tensorrt_sample

### How to run this saample
1. As Torch-TensorRT already integrated into NGC pytorch docker image, you can use it directly through the NGC docker image like 'nvcr.io/nvidia/pytorch:21.11-py3'

    If you use server to run this sample, you can map the notebook port to host by following steps:
   
    a. start a docker: docker run --rm -it --gpus '"device=0"' -v /home/yongming/:/workspace/hostdir -p 8889:8888 nvcr.io/nvidia/pytorch:21.11-py3
   
    b. clone the sample:  
   start a 