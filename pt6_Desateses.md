Instal·lació del isomaster
Utilitzo la seguent comanda


*** Enlloc de l’isomaster es pot fer ús de rsync per a extreure tot lo de la iso i desprès mkisofs per a tornar a generar-la

Realitza la instal·lació desatesa amb el kickstart d'un SO Ubuntu
Actualitza repositoris


Instal·la system-config-kickstart



Obre amb system-config-kickstart i configura els paràmetre que creguis necessaris




He modificat el idioma default a catala, el teclat a l’español i la hora

Marco l’opcio utilitzar GRUP password i encriptar 


Aqui fico les particions

Fico la ip estatica


Creo l’usuari oriol


Fico el color 24 i la resolucio 1280x1024

Selecciono Kubuntu Desktop






Guarda l’arxiu ks.cfg a l’escritori mateix
Guardo l’arxiu ks.cfg a l’escritori

Li dono tots el permisos per a poder modificar-ho


Obre la .iso alternate o server amb l’isomaster i posa a l’arrel l’arxiu ks.cfg



Agrego el ks.cfg


Amb l’isomaster extreu l’arxiu txt.cfg a l’escritori mateix, i modifca’l per tal d’afegir una opció més al menú. Copia la primera opció, caniva el nom i afegeix al final ks=cdrom:/ks.cfg
Extrec el txt.cfg per a modificar-ho


Guarda els canvis
He canivat el menu label i el quiet

Posa aquets arxiu modificat dintre la iso, esborrant primer l’antic



Guarda la iso
Guardo la iso amb el nom OriolDesates

Prova que funcioni en una nova màquina virtual

Realitza la instal·lació desatesa amb el pressed d'un SO Ubuntu. El concepte és el mateix, generar un arxiu de resposta, però enlloc del kickstart amb el pressed i desprès posar-lo dintre la iso.
Cerca per internet un arxiu preseed.cfg i modifica’l
Llavors cal que el posis dintre la iso i que modifiquis el txt.cfg afegint una nova opció per a que l’agafi
Extrec el cfg


Li dono permisos per a modificar-ho

Canvio el append

https://www.pugetsystems.com/labs/hpc/note-auto-install-ubuntu-with-custom-preseed-iso-1654/

Elimino el cfg antic i fico el nou modificat


Guardo la nova iso amb el nom OriolDesatesa2

Prova la iso en una nova màquina virtual
