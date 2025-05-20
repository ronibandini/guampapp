![guampapp2](https://github.com/user-attachments/assets/d5b0c2e1-1ed3-4756-bb3d-3ceed112fc35)

# Guampapp (no es una app)
Dispositivo con IA para determinar infidelidades 
Mayo de 2025, MIT License

# Partes requeridas
Cámara AI Cam ESP32S3 de DF Robot [https://wiki.dfrobot.com/SKU_DFR1154_ESP32_S3_AI_CAM#target_5](https://www.dfrobot.com/product-2899.html?tracking=hOuIhw4fDaJRTdy4abz04npbQC78dqxBkqVt7XMFYxEXj2s0ukWgm71wbut0ewUP)
2 partes impresas en 3D https://cults3d.com/en/3d-model/tool/guamp-app

# Instrucciones
Entrenar un modelo en Edge Impulse y hacer Deploy como Arduino Library (asimismo es posible usar el modelo entrenado para reconocer personas)

1. Copiar el zip a "Documents/arduino/libraries" 
2. Reemplazar "depthwise_conv.cpp" y "conv.cpp" en "src\edge-impulse-sdk\tensorflow\lite\micro\kernels" del zip exportado por los archivos del mismo nombre incluidos en https://dfimg.dfrobot.com/5d57611a3416442fa39bffca/wiki/074b3c8aa70b013bdc7c4b39babd03b1.zip 
3. Mover la carpeta edge_camera y sus subcarpetas a Documents/arduino/libraries/modelFolder/examples  
4. Abrir el Arduino IDE, seleccionar el ejemplo de edge_camera, modificar la primera línea para que indique el .h del modelo. Ejemplo:
	#include <Person_Detection_inferencing.h>

5. Seleccionar en Arduino IDE la placa ESP32S3 Dev Module
6. Seleccionar los seteos como OPI Psram, 16mg Flash, etc Detalles de esto en https://wiki.dfrobot.com/SKU_DFR1154_ESP32_S3_AI_CAM#target_5
7. Cargar SSID, pass, Telegram token, openAI token, etc
8. Upload

# Contacto
Roni Bandini
https://www.instagram.com/ronibandini/
