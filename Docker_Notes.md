# Instructions for tf-retinanet to install and run

apt install -y libsm6 libxext6 libxrender1
pip install opencv-python Pillow progressbar2 dill pyyaml
python setup.py build_ext --inplace
python setup.py develop --user
cd ..
git clone https://github.com/Jakedismo/tf-retinanet-backbones-resnet50v2.git
git clone https://github.com/Jakedismo/tf-retinanet-backbones-resnet101v2.git
git clone https://github.com/Jakedismo/tf-retinanet-backbones-resnet152v2.git
git clone https://github.com/fizyr/tf-retinanet-backbones-resnet.git
git clone https://github.com/Jakedismo/tf-retinanet-generators-csv.git
git clone https://github.com/fizyr/tf-retinanet-generators-coco.git

for each of these do:

python setup.py develop --user

