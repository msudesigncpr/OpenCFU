# OpenCFU

## About
OpenCFU is a `C++` program originally used to enumerate colonies through a GUI. 
[libcolonyfind](https://github.com/msudesigncpr/libcolonyfind/tree/main) relies heavily on this program to function. See the [libcolonyfind docs](https://msudesigncpr.github.io/libcolonyfind/libcolonyfind/colony_finder.html) for more info. 
Because OpenCFU cannot properly parse command-line arguments in Windows, OpenCFU must be 
built in `WSL` and invoked from Windows. 

See the [datasheets](https://github.com/msudesigncpr/datasheets/tree/tonic) for the OpenCFU reference paper
## Installation
(All in `WSL`)

> install opencv devel ver
```
sudo apt update && apt install libopencv-dev
```
> clone into OpenCFU
```
git clone https://github.com/msudesigncpr/OpenCFU.git
```
> build
```
cd OpenCFU
```
```
autoreconf -i
```
```
./configure --without-gui
```
```
automkae --add-missing
```
```
./opencfu -h
```

Define this path in [constants.py](https://github.com/msudesigncpr/libcolonyfind/blob/main/src/libcolonyfind/constants.py)


[Docs ](https://msudesigncpr.github.io/libcolonyfind/libcolonyfind/constants.html)for more info
