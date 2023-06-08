Recursos necessaris:
-Màquina base amfitrió Ubuntu 14.04, Ubuntu 16.04...
-Alguna .iso versió alternate o server DINTRE de la MV amfitrió
-Instal·lació del isomaster
Utilitzo la seguent comanda

![Selecció_1024](https://github.com/omarine12/MP05/assets/113585932/1197a413-d6b8-478b-8a87-d80fb93534c4)


*** Enlloc de l’isomaster es pot fer ús de rsync per a extreure tot lo de la iso i desprès mkisofs per a tornar a generar-la

Realitza la instal·lació desatesa amb el kickstart d'un SO Ubuntu
Actualitza repositoris

![Selecció_1025](https://github.com/omarine12/MP05/assets/113585932/cfae3da0-a5e0-4b7d-9ac5-763bf645b9d3)


Instal·la system-config-kickstart

![Selecció_1026](https://github.com/omarine12/MP05/assets/113585932/223a6d68-05f8-45e0-adb9-a77ede8df236)


Obre amb system-config-kickstart i configura els paràmetre que creguis necessaris


![Selecció_1028](https://github.com/omarine12/MP05/assets/113585932/ad4f64d6-acac-4c4d-8715-e0b8f798b100)


He modificat el idioma default a catala, el teclat a l’español i la hora

![Selecció_1029](https://github.com/omarine12/MP05/assets/113585932/1c7f6444-c49f-4b10-9010-bedb9f2cd606)


Marco l’opcio utilitzar GRUP password i encriptar 

![Selecció_1031](https://github.com/omarine12/MP05/assets/113585932/b120dd08-8e48-47aa-8cf1-689ca0f048f0)

Aqui fico les particions

![Selecció_1032](https://github.com/omarine12/MP05/assets/113585932/ef62d30f-b4c6-4fd2-9a49-afa724c4cceb)

Fico la ip estatica

![Selecció_1033](https://github.com/omarine12/MP05/assets/113585932/6aae4cca-4c58-428d-8968-69ce5a9c34e1)


Creo l’usuari oriol

![Selecció_1034](https://github.com/omarine12/MP05/assets/113585932/1ab6511c-2950-4482-a63c-3ad79aa28a68)

Fico el color 24 i la resolucio 1280x1024

![Selecció_1036](https://github.com/omarine12/MP05/assets/113585932/51e0f540-a4ec-4cbb-a1bf-4fb09f784734)

Selecciono Kubuntu Desktop

![Selecció_1037](https://github.com/omarine12/MP05/assets/113585932/1b2d1250-ae2c-4404-ad11-4f1cc8238a1c)

Guarda l’arxiu ks.cfg a l’escritori mateix
Guardo l’arxiu ks.cfg a l’escritori

![Selecció_1038](https://github.com/omarine12/MP05/assets/113585932/2fb66f38-81ba-4a7e-8e8c-34626f340e82)

Li dono tots el permisos per a poder modificar-ho

![Selecció_1039](https://github.com/omarine12/MP05/assets/113585932/a95570b8-3d22-4837-8ffb-e748593d2bd3)

Obre la .iso alternate o server amb l’isomaster i posa a l’arrel l’arxiu ks.cfg

![Selecció_1040](https://github.com/omarine12/MP05/assets/113585932/b080efc6-bafb-4da4-9ce1-1a2b3ec13fa5)


Agrego el ks.cfg

![Selecció_1041](https://github.com/omarine12/MP05/assets/113585932/e9cbf476-64bd-4f5d-82b3-ac24819a15ba)


Amb l’isomaster extreu l’arxiu txt.cfg a l’escritori mateix, i modifca’l per tal d’afegir una opció més al menú. Copia la primera opció, caniva el nom i afegeix al final ks=cdrom:/ks.cfg
Extrec el txt.cfg per a modificar-ho

![Selecció_1042](https://github.com/omarine12/MP05/assets/113585932/871d385f-9fe4-4976-ba85-8ce1ea52ba10)


Guarda els canvis
He canivat el menu label i el quiet

![Selecció_1043](https://github.com/omarine12/MP05/assets/113585932/da20e22f-01bf-495d-a4c8-29bb56e28227)


Posa aquets arxiu modificat dintre la iso, esborrant primer l’antic

![image](https://github.com/omarine12/MP05/assets/113585932/b861aa62-81af-4db0-8158-21b74c526158)



Guarda la iso
Guardo la iso amb el nom OriolDesates

![Selecció_1045](https://github.com/omarine12/MP05/assets/113585932/ccc59bfc-abd3-4e41-b0d6-30578219ba40)


j.Prova que funcioni en una nova màquina virtual

![Selecció_1053](https://github.com/omarine12/MP05/assets/113585932/c7dac6a5-9f59-4ed6-afbd-9d2f0310f0c9)

![image](https://github.com/omarine12/MP05/assets/113585932/85199fad-88b1-4a5d-a0ff-8f47db9d16ad)

![image](https://github.com/omarine12/MP05/assets/113585932/5d02acfe-9496-48b8-8a17-4a6e66e47731)

![image](https://github.com/omarine12/MP05/assets/113585932/67ea366a-8622-4697-9f68-50c4131d72a2)

![image](https://github.com/omarine12/MP05/assets/113585932/2065932d-cdaf-49fe-b25a-51afe5171952)

![image](https://github.com/omarine12/MP05/assets/113585932/8617e7a3-bc94-4649-a3bc-af5c7194761d)

![image](https://github.com/omarine12/MP05/assets/113585932/10095daa-8c85-4221-8c76-a2629212d8ba)

![image](https://github.com/omarine12/MP05/assets/113585932/6ef59b74-ae6a-4935-b625-5d218e933542)


2.Realitza la instal·lació desatesa amb el pressed d'un SO Ubuntu. El concepte és el mateix, generar un arxiu de resposta, però enlloc del kickstart amb el pressed i desprès posar-lo dintre la iso.
Cerca per internet un arxiu preseed.cfg i modifica’l
Llavors cal que el posis dintre la iso i que modifiquis el txt.cfg afegint una nova opció per a que l’agafi
Extrec el cfg

![image](https://github.com/omarine12/MP05/assets/113585932/73733a96-be19-4d7f-84b3-1f14b1216548)

Li dono permisos per a modificar-ho

![Selecció_1049](https://github.com/omarine12/MP05/assets/113585932/5028e46a-6949-4dca-9398-9016286fe2a8)


Modifico el append

![Selecció_1050](https://github.com/omarine12/MP05/assets/113585932/0269bcfd-01fc-4262-afd7-08a32f445ac7)

Aqui he tret tota la informació
https://www.pugetsystems.com/labs/hpc/note-auto-install-ubuntu-with-custom-preseed-iso-1654/

Elimino el cfg antic i fico el nou modificat

![Selecció_1051](https://github.com/omarine12/MP05/assets/113585932/4ecf8e23-4616-4bcd-ba15-c9496227bd34)


Guardo la nova iso amb el nom OriolDesatesa2
![Selecció_1052](https://github.com/omarine12/MP05/assets/113585932/8caa367c-a5d8-47bd-a54a-9b8aa020fe5b)
Prova la iso en una nova màquina virtual
Mostro com s'instal·la automaticament
![image](https://github.com/omarine12/MP05/assets/113585932/6829ac8a-26f8-424a-a377-a58a8a63d5d5)

![image](https://github.com/omarine12/MP05/assets/113585932/21c41883-c44f-4d6b-a0eb-6618464ca373)

![image](https://github.com/omarine12/MP05/assets/113585932/63c3d0a6-58b7-4d26-a213-4094f3503eb6)

![image](https://github.com/omarine12/MP05/assets/113585932/09af2b65-f435-4383-a938-ff3bd7d994fb)

![image](https://github.com/omarine12/MP05/assets/113585932/69415d38-ebf3-428c-90c6-9ee3b75862ff)

![image](https://github.com/omarine12/MP05/assets/113585932/0a956ae9-980b-4862-95cd-ab94cc630993)
