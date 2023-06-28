

# install

``` bash

export AM_I_DOCKER=False
export BUILD_WITH_CUDA=True
export CUDA_HOME=/usr/local/cuda-11.8/

pip install -e segment_anything -i https://pypi.tuna.tsinghua.edu.cn/simple
pip install -e GroundingDINO  -i https://pypi.tuna.tsinghua.edu.cn/simple
pip install --upgrade diffusers[torch] -i https://pypi.tuna.tsinghua.edu.cn/simple
pip install opencv-python pycocotools matplotlib onnxruntime onnx ipykernel  -i https://pypi.tuna.tsinghua.edu.cn/simple

git submodule update --init --recursive

cd grounded-sam-osx && bash install.sh

cd Tag2Text && pip install -r requirements.txt

```

# dmeo
```bash
CUDA_VISIBLE_DEVICES=5 python grounded_sam_simple_demo.py

```