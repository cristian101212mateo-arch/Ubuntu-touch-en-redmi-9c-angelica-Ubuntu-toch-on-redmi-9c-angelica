# Ubuntu-touch-en-redmi-9c-angelica-Ubuntu-toch-on-redmi-9c-angelica
Quiero aclarar que no lo compile sino solo doy los pasos de como se instala 
Paso 1: tener miui 22.0.10 dejo el link https://mifirm.net/download/4733
Paso 2 :Descargar el devel-flasheable que puse en el repo 
Paso 3: descargar el vmeta disable es obligatotio 
Ya aclarando esto primero ay que entrar a fastboot 
en fastboot primero flaseamo el recovery del devel-flashable con: fastboot flash recovery recovery.img 
para despues:
gastboot reboot fastboot 
despues que esten en fastbootd ayque borar product con este comando :fastboot delete-logical-partition product
despues flaseamos el system con : fastboot flash system system.img 
y luego flashear el boot con: fastboot flash boot boot.im
y por utilmo flashear el vmeda_disable
fastboot flash vbmeta vbmeta_disabled.img

fastboot flash vbmeta_system vbmeta_disabled.img

fastboot flash vbmeta_vendor vbmeta_disabled.img

Para terminar un fastboot reboot 


Nota si aparese poco espasio as un format data desde el recovery

Perdon si quedo mal es mi priner repo en github
