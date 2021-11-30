## torch-tensorrt_sample

### How to run this sample
1. As Torch-TensorRT already integrated into NGC pytorch docker image, you can use it directly through the NGC docker image like 'nvcr.io/nvidia/pytorch:21.11-py3'

    If you use server to run this sample, you can map the notebook port to host by following steps:
   
    a. start a docker: `docker run --rm -it --gpus '"device=0"' -v /home/yongming/:/workspace/hostdir -p 8889:8888 nvcr.io/nvidia/pytorch:21.11-py3`
   
    b. clone the sample: `git clone https://github.com/shiyongming/torch-tensorrt_sample.git`
   
    c. start a notebook: `jupyter notebook --ip=0.0.0.0 --NotebookApp.token='' --no-browser --port=8888 --allow-root`

2. on your windows notebook tap win+r and run cmd
3. In cmd window run ssh -N -f -L `localhost:8889:localhost:8888 -p 22 username@server_ip_address`. Please change the username and ip address.
4. open a browser amd enter `localhost:8889` 