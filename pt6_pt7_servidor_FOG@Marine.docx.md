# Servidor d’Imatges

## 1. Instal·lar i configurar un servidor FOG

Primer descarrego el fog desde la pàgina web
![Selecció_976](https://github.com/omarine12/MP05/assets/113585932/86a42610-ecfe-4734-b269-33d9c554b7b3)

Despres descomprimeixo el paquet tar.gz

![Selecció_977](https://github.com/omarine12/MP05/assets/113585932/8e59bc74-b8bd-4750-8461-87d08f3cd7d1)

Entro a la carpeta del fog i executo la instalacio

![image](https://github.com/omarine12/MP05/assets/113585932/28f7d41f-6d3d-4a22-9642-6a3514691907)

Aquest son les opcions i els parametres que he ficat a l’instalacio
![image](https://github.com/omarine12/MP05/assets/113585932/81bb98de-3970-4669-953e-843638bf394d)

Per finalitzar l’instalacio, al navegador donarem clic al botó instalar
![image](https://github.com/omarine12/MP05/assets/113585932/3dc9af6e-0116-42aa-b743-77b61fb8a995)

Per entrar al fog tindre que utilitzar la ip de la maquina, aquestes son les credencials per a entrar
![image](https://github.com/omarine12/MP05/assets/113585932/7a62b721-9da3-4a68-882a-68ddfc1cda2e)

Fico la ip al navegador i entro
![image](https://github.com/omarine12/MP05/assets/113585932/05175f97-79b9-43ee-a2bc-94d2d3c5e20c)

Aquest es el menu principal del fog
![image](https://github.com/omarine12/MP05/assets/113585932/9f68df2b-09cb-45c2-b5c6-9462391b7525)

Deshabiliitem el proces system-resolved
![image](https://github.com/omarine12/MP05/assets/113585932/292bfdc2-122e-4cbf-aa40-32c362041fb1)


Aturem el proces i borrem l’arxiu resolv.conf i el tornem a crear amb el nameserver 8.8.8.8

Instal·lem el dnsmasq per a direccionar els clients al nostre FOG
![image](https://github.com/omarine12/MP05/assets/113585932/a4754fce-3439-48d9-8f94-ef812c36d3f0)

Fiquem els seguents parametres dins de l’arxiu /etc/dnsmasq/ltsp.conf

- port=0
- log-dhcp
- tftp-root=/tftpboot
- dhcp-no-override
- dhcp-boot=undionly.kpxe,,192.168.204.226
- pxe-prompt="Booting FOG Client", 1
- dhcp-range=192.168.204.226,proxy
![image](https://github.com/omarine12/MP05/assets/113585932/add3ecc3-c56b-41ba-be17-ab2b1c1d7f1a)


Gurado els canvis i reinicio el dnsmasq
![image](https://github.com/omarine12/MP05/assets/113585932/5b3ba451-70f0-4369-84ce-ecfc3f6b0af3)


## 2. Capturar des del client un Windows

Creem una imatge desde el fog i iniciem la maquina desde la xarxa, desprès registrem el host
![image](https://github.com/omarine12/MP05/assets/113585932/7bc5e650-78a0-4f4d-9452-5ada6a265397)

Un cop registrada exportem la imatge
![image](https://github.com/omarine12/MP05/assets/113585932/9f2c4092-dbf4-440c-9609-a193968db03a)

A l’apartat de tasques basiques si tot ha funcionat correctament ens dira que la tasca s’ha completat correctament
![image](https://github.com/omarine12/MP05/assets/113585932/e2083195-08dc-4652-894a-c0aac4922f83)


A **image Managemet** podrem veure la imatge clonada correctament
![image](https://github.com/omarine12/MP05/assets/113585932/f91729f9-b5db-49fc-a17e-17bf11ad0581)



## 3. Capturar des del client un Ubuntu

Primer instal·lo 2 aplicacions per a fer les comprovacions un cop finalitzat (**discord i krita**)
![image](https://github.com/omarine12/MP05/assets/113585932/b6e06dc1-2b6d-420c-824c-1bdd5d2594fc)


Primer creem una nova imatge, establim el **nom, la descripcio(opcional), sistema operatiu i la ruta de l’imatge**
![image](https://github.com/omarine12/MP05/assets/113585932/eb3b1ffc-5e50-4e1d-94f8-e80b9c0a90ed)

Entrem amb la xarxa i registrem el host
![image](https://github.com/omarine12/MP05/assets/113585932/04773058-3cba-47ed-b0fe-9950be4e8f62)


Desde el **Host Management**, es pot veure com s’ha registrat correctament el host
![image](https://github.com/omarine12/MP05/assets/113585932/f42524bf-9631-4f04-ae57-955cd9e0d111)

Dins de **Host general** canviarem el nom, enllaçem l’imatge que hem creat abans amb aquest host
![image](https://github.com/omarine12/MP05/assets/113585932/e64e1bad-f962-41b4-bf40-f885c08619be)

Desprès anem a **capture, basik task** i li donem a **task**
![image](https://github.com/omarine12/MP05/assets/113585932/75cff8b3-0364-46bf-9225-fb3681b027a3)


Si la tasca ha funcionat be la podrem guardar
![image](https://github.com/omarine12/MP05/assets/113585932/d385fc85-43ab-4ddd-a3ab-fd281e990e45)

A **Imatge Management** es pot veure la imatge clonada
![image](https://github.com/omarine12/MP05/assets/113585932/c24f4a54-40c0-4af0-9fe7-dd5688b14ae8)


## 4. Instal·lar imatge Windows

Creem una maquina virtual sense cap sistema operatiu i entrem per xarxa, despres seleccionem l’opcio **Deploy Image**
![image](https://github.com/omarine12/MP05/assets/113585932/5cf72bd2-94d7-4d5b-918a-a60124a472bc)

Fiquem les **creedencials** del nostre fog
![image](https://github.com/omarine12/MP05/assets/113585932/41ab67f9-87d8-46ea-9011-e1575aaf337c)

Quan accedim podrem seleccionar,l’imatge de Windows 10
![image](https://github.com/omarine12/MP05/assets/113585932/6dafe4f1-eca6-4687-a1fe-45641dc34c8e)

Tenim que esperar a que es desplegui la imatge al client
![image](https://github.com/omarine12/MP05/assets/113585932/d7f04eae-17a5-42f6-910b-abe4f30ad7d3)


Un cop finalitzat podem encendre la maquina i comrpovar que la imatge s’ha establert correctament

![image](https://github.com/omarine12/MP05/assets/113585932/2dda4fcb-97a5-4b67-aadc-831141e31b04)




## 5. Instal·lar imatge Ubuntu

Creo la maquina virtual **FOG Instalar Ubuntu** sense cap imatge i entro per xarxa, despres seleciono l’opcio deploy image
![image](https://github.com/omarine12/MP05/assets/113585932/f733837e-51e7-4671-9f95-eb5059b31350)

Escric les credencials correctament
![image](https://github.com/omarine12/MP05/assets/113585932/f03c47fa-02ab-415a-8e4d-6f89f125ce63)

Selecciono l’imatge d’ubuntu que he creat anteriorment
![image](https://github.com/omarine12/MP05/assets/113585932/53bef4c3-76a9-48e9-8dee-4c7ee04aee12)


Tenim que esperar a que es desplegui l’imatge
![image](https://github.com/omarine12/MP05/assets/113585932/09f77964-de7f-4b9e-ba0b-6c8e2bcb8106)

Un cop descarregada es pot veure com els 2 programes que he instalat anteriorment estan a l’imatge instalada, i a la maquina **FOG Instalar Ubuntu**
![image](https://github.com/omarine12/MP05/assets/113585932/bf9d7db1-cc14-4808-8dc9-0d646b676237)


## 6. Llençar un paquet per a que s’instal·li als clients

Anem a l’apartat de **snaping** i creem un nou complement, amb un **nom i la msi de google chrome**
![image](https://github.com/omarine12/MP05/assets/113585932/52edb2c8-312b-4284-9c75-948b70641de1)

Desprès inicio un client windows amb xarxa, i selecciono l’opcio **Quick Registration and Inventory** per registtrar el client com a host


Entro a editar host i selecciono la casella per veure snapings que poden ser afegits, selecciono google chrome

Despres vaig a l’apartat de **host task i advanced**
![image](https://github.com/omarine12/MP05/assets/113585932/fe108f35-a2b9-44d8-ac1c-4ec24f2df749)


Es pot veure com s’ha creat correctament


A l’apartat de **FOG CLIENT,** seleccionem l’opcio smart installer


Quan li donem s’obrira una pestanya on tenim que ficar la **IP DEL SERVIDOR**

Si funciona correctament ens saltara una notificacio dient que **s’esta instalant i que s’ha instalat correctament**



El fog ens informa que hem de **reiniciar la maquina**


I es pot veure com al reinciciar **s’ha instalat el chrome.**

