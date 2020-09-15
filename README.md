# Pytorch Raspberry Pi builds
Unofficial RPi Pytorch and torchvision builds

## Building your own wheel
First build pytorch or vision from scratch. I found this [guide](https://blog.openmined.org/federated-learning-of-a-rnn-on-raspberry-pis/) particularly useful.

After confirming that the pip package works, we can now build a wheel using the following command:
```
sudo -E python3 setup.py bdist_wheel
```
After this you'll find the wheel in the _dist/_ folder.

## Installing downloaded wheels
Clone this repository and install using the name of the wheel. E.g.
```
pip install torch-1.6.0a0+b31f58d-cp38-cp38-linux_armv7l.whl
```