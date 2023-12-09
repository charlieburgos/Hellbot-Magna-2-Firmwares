/# Hellbot-Magna-2-Firmwares
Firmwares para todas las mag/na 2 230/300/400/500

Desarrollo de Marlin para las diferentes main. 
Actualmente 27/06/2023 MKS Robin Nano v1.3 no bltouch disponible. Stable
-----
Actualizacion 19/10/2023 Marlin 2.1.2.1 RN13 BLtouch disponible. Stable

-----

Actualización 09/12/2023

Ajuste de microstep para silenciar un poco mas al momento de imprimir. 

------

Se incorpora firmware que permite uso de Bucket Purge, al extender en 30 la distancia del eje X. 
Mayores detalles de Bucket Purge aqui :  https://www.youtube.com/watch?v=r9yTyyXRF-U

Se agrega firmware  que  modifica en la main el sensado de temperatura de hotend. de TH1 a Th2, para quienes tienen daño en la main con el th1. 

Terminologia 

NOBLT = Sin Bltouvh
BP = Bucket Purge 
BLT = BlTouch
TH2 = usa termistor 2 como si fuera th1
HE1 = usa terminal de la placa  He1 para calentar hotend, y th2 para sensar para quienes tienen dañado el mosfet y esta siempre calentando o no calienta. 
