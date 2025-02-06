# bsp example hello


## from git code

https://github.com/espressif/esp-bsp/tree/master/examples

```
#add demo to the helloworld example:
helloWorld$ mkdir components
cp -ar ../esp-bsp/examples/display_camera/ components/

```

## from new blank project

```
idf.py create-project XXXX
# then cd and :  idf.py add-dependency "espressif/XXXX"
```


## from registry

find and do:  idf.py add-dependency "espressif/XXXX"