# Casco inteligente de motociclista
Modelos de detección de objetos y segmentación de imagen utilizados en el proyecto SISTEMA DE DETECCIÓN Y VISUALIZACIÓN DE VEHÍCULOS MEDIANTE VISIÓN ARTIFICIAL PARA CASCO DE MOTOCICLISTA. Los códigos son compatibles con Raspberry Pi 4 B y Raspberry Pi OS Kernel version: 5.4

## Detección de objetos
Los modelos están optimizados para ser ejecutados en Raspberry Pi, basados en la arquitectura MobileNet V3.

### Ejecución  Raspberry Pi Camera
python3 detect_pi.py \
  --model model_1.tflite \
  --labels coco_labels.txt

Para probar la ejecución con otro modelo cambiar el nombre al llamar en consola.

### Inferencia en video
python3 classify_picamera.py \
  --graph model_1.tflite \
  --labels coco_labels.txt \
  -- video video_trafico.mp4

## Segmentación de imagen
