![guampapp2](https://github.com/user-attachments/assets/d5b0c2e1-1ed3-4756-bb3d-3ceed112fc35)

# Guampapp (no es una app)
Dispositivo con IA para determinar infidelidades 
Mayo de 2025, MIT License

# Partes requeridas
Cámara AI Cam ESP32S3 de DF Robot [https://wiki.dfrobot.com/SKU_DFR1154_ESP32_S3_AI_CAM#target_5](https://www.dfrobot.com/product-2899.html?tracking=hOuIhw4fDaJRTdy4abz04npbQC78dqxBkqVt7XMFYxEXj2s0ukWgm71wbut0ewUP)
2 partes impresas en 3D https://cults3d.com/en/3d-model/tool/guamp-app

# Instrucciones
Estas instrucciones contemplan la instalación de un modelo para detección de personas. En https://www.hackster.io/roni-bandini/guampapp-with-esp32s3-ai-camera-module-cc7f91 es posible ver cómo entrenar un modelo con fotos propias.

. Desde el Arduino IDE agregar la librería https://github.com/ronibandini/guampapp/blob/main/PersonDetectionInferencing.zip
. Seleccionar la placa ESP32S3 Dev Module
. Configurar los seteos de OPI Psram, 16mg Flash, etc Detalles de esto en https://wiki.dfrobot.com/SKU_DFR1154_ESP32_S3_AI_CAM#target_5
. Cargar SSID, pass, Telegram token, openAI token en el código .ino
. Subir al AI Module

# Video
https://www.youtube.com/shorts/LsQOEmBrbVo

# Contacto
Roni Bandini
https://www.instagram.com/ronibandini/
