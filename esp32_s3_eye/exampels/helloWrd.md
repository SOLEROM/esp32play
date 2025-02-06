# hello world

```
> cp -ar ../esp/esp-idf/examples/get-started/hello_world/* . 

```

```

> idf.py set-target esp32s3

-- Build files have been written to: /home/user/proj/s3eye/helloWorld/build

helloWorld/build
├── app-flash_args
├── bootloader
├── bootloader-flash_args
├── bootloader-prefix
├── build.ninja
├── CMakeCache.txt
├── CMakeFiles
├── cmake_install.cmake
├── compile_commands.json
├── config
├── config.env
├── esp-idf
├── flash_app_args
├── flash_args
├── flash_args.in
├── flash_bootloader_args
├── flasher_args.json
├── flash_project_args
├── kconfigs.in
├── kconfigs_projbuild.in
├── ldgen_libraries
├── ldgen_libraries.in
├── log
├── partition-table-flash_args
└── project_description.json

```


```
> idf.py menuconfig

```

```
> idf.py build

Project build complete. To flash, run:
 idf.py flash
or
 idf.py -p PORT flash
or
 python -m esptool --chip esp32s3 -b 460800 --before default_reset --after hard_reset write_flash --flash_mode dio --flash_size 2MB --flash_freq 80m 0x0 build/bootloader/bootloader.bin 0x8000 build/partition_table/partition-table.bin 0x10000 build/hello_world.bin
or from the "/home/user/proj/s3eye/helloWorld/build" directory
 python -m esptool --chip esp32s3 -b 460800 --before default_reset --after hard_reset write_flash "@flash_args"


```


### tree

```
.
├── build
│   ├── app-flash_args
│   ├── bootloader
│   ├── bootloader-flash_args
│   ├── bootloader-prefix
│   ├── build.ninja
│   ├── CMakeCache.txt
│   ├── CMakeFiles
│   ├── cmake_install.cmake
│   ├── compile_commands.json
│   ├── config
│   ├── config.env
│   ├── esp-idf
│   ├── flash_app_args
│   ├── flash_args
│   ├── flash_args.in
│   ├── flash_bootloader_args
│   ├── flasher_args.json
│   ├── flash_project_args
│   ├── hello_world.bin
│   ├── hello_world.elf
│   ├── hello_world.map
│   ├── kconfigs.in
│   ├── kconfigs_projbuild.in
│   ├── ldgen_libraries
│   ├── ldgen_libraries.in
│   ├── log
│   ├── partition_table
│   ├── partition-table-flash_args
│   ├── project_description.json
│   ├── project_elf_src_esp32s3.c
│   └── x509_crt_bundle.S
├── CMakeLists.txt
├── main
│   ├── CMakeLists.txt
│   └── hello_world_main.c
├── pytest_hello_world.py
├── README.md
├── sdkconfig
└── sdkconfig.ci

```