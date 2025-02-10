# dockerize

use docker to build esp32s3eye

```
start img:
        616M    /save/esp32s3eye_docker_image.tar
after install:
        7.6G   /save/esp32s3eye_docker_image.tar
```


## build

```
mkdir /home/user/esp-idf /home/user/IDF_TOOLS_PATH
git clone -b v5.4 --recursive https://github.com/espressif/esp-idf.git .
cd esp-idf
export IDF_TOOLS_PATH="/home/user/IDF_TOOLS_PATH"
./install.sh esp32s3
. ./export.sh


git clone https://github.com/espressif/esp-who.git
git clone https://github.com/espressif/esp-bsp.git
git clone https://github.com/espressif/esp-nn
git clone https://github.com/espressif/esp-tflite-micro.git
```

# run
        cd /home/user/esp-idf
        export IDF_TOOLS_PATH="/home/user/IDF_TOOLS_PATH"
        . ./export.sh

