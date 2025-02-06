# hello tflite

```
> idf.py create-project helloTFlite

> idf.py add-dependency "esp-tflite-micro"
Executing action: add-dependency
NOTICE: Created "/home/user/proj/s3eye/demos/helloTFlite/main/idf_component.yml"
NOTICE: Successfully added dependency "espressif/esp-tflite-micro": "*" to component "main"
NOTICE: If you want to make additional changes to the manifest file at path /home/user/proj/s3eye/demos/helloTFlite/main/idf_component.yml manually, please refer to the documentation: https://docs.espressif.com/projects/idf-component-manager/en/latest/reference/manifest_file.html
Done

```

```
main/idf_component.yml 
=======================
## IDF Component Manager Manifest File
dependencies:
  ## Required IDF version
  idf:
    version: '>=4.1.0'
  # # Put list of dependencies here
  # # For components maintained by Espressif:
  # component: "~1.0.0"
  # # For 3rd party components:
  # username/component: ">=1.0.0,<2.0.0"
  # username2/component2:
  #   version: "~1.0.0"
  #   # For transient dependencies `public` flag can be set.
  #   # `public` flag doesn't have an effect dependencies of the `main` component.
  #   # All dependencies of `main` are public by default.
  #   public: true
  espressif/esp-tflite-micro: '*'                   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

```

## examples on repo:

```
esp-tflite-micro/examples/
├── hello_world
├── micro_speech
└── person_detection
```