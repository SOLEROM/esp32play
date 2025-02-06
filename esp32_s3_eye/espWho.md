# Esp WHO

* contain default prebuild FW :    esp-who/default_bin/esp32-s3-eye/

allows you to test its functions including voice wake-up, voice command recognition, face detection and recognition.

projects

```
├── human_face_detect
├── human_face_detect_lvgl
├── human_face_recognition
├── pedestrian_detect
└── pedestrian_detect_lvgl
```

run

```
  idf.py set-target esp32s3
  idf.py menuconfig
  idf.py build
  idf.py flash
```