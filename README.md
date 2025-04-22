# Proyecto en raspberry con scratch

Se ha realizado un proyecto que sirve para detectar alcohol con un sensor de alcohol analógico (QM3)  
Lo primero que se va a detallar, son las conexiones  

![conexiones](/img/WhatsAppImage2025-04-22at11.19.06.jpeg)  
El sensor cuenta con 4 pines, de los cuales se utilizaran solo 3, VCC, GND y D0  
La conexión que se lleva a cabo es la siguiente:  
VCC->5V  
GND->GND  
DO->GPIO 17  

Una vez se ha realizado la conexión, lo siguiente es el código:  

Si GPIO 17 se encuentra en HIGH, significa que no se está detectando alcohol, por lo que imprime en pantalla un mensaje que dice "Alcohol no detectado"  
Si por el contrario se encuentra en LOW, significará que está detectando alcohol, por ende imprime por pantalla un mensaje que dicta "Alcohol detectado"  

Aunque el sensor es analógico, es necesario una controladora para poder tomar esa entrada analógica. Debido a esto, se trata la entrada como digital (HIGH y LOW)
