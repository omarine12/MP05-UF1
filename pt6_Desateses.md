> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image4.png){width="12.354166666666666in"
> height="7.721353893263342in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic

+-----------------------------------------------------------------------+
| > **Instal·lació desatesa amb fitxer de resposta**                    |
+=======================================================================+
+-----------------------------------------------------------------------+

> Per a fer una instal·lació desatesa amb Ubuntu existeixen dues
> opcions, la primera és fer-ho amb el kickstart, la qual té l'avantatja
> que és més senzilla d'utilitzar, però és menys completa. L'altra és
> amb el preseed, és més complexa, però la configuració és molt més
> extensa.
>
> Recursos necessaris:
>
> ● Màquina base amfitrió Ubuntu 14.04, Ubuntu 16.04\...
>
> ● Alguna .iso versió alternate o server **DINTRE** de la MV amfitrió ●
> Instal·lació del isomaster\
> Utilitzo la seguent comanda
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image1.png){width="5.301388888888889in"
> height="1.1569444444444446in"}
>
> **\*\*\* Enlloc de l'isomaster es pot fer ús de rsync per a extreure
> tot lo de la iso i desprès mkisofs per a tornar a generar-la**
>
> 1\. Realitza la instal·lació desatesa amb el kickstart d\'un SO Ubuntu
> a. Actualitza repositoris

![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image2.png){width="7.270833333333333in"
height="0.8222211286089239in"}

> b\. Instal·la system-config-kickstart
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image3.png){width="6.781943350831146in"
> height="1.3430544619422573in"}
>
> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image7.png){width="12.354166666666666in"
> height="5.821718066491688in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic

+-----------------------------------+-----------------------------------+
| c\.                               | > Obre amb                        |
|                                   | > system-config-kickstart i       |
|                                   | > configura els paràmetre que     |
|                                   | > creguis necessaris              |
+===================================+===================================+
+-----------------------------------+-----------------------------------+

> He modificat el idioma default a catala, el teclat a l'español i la
> hora
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image5.png){width="3.9583333333333335in"
> height="3.0625in"}
>
> Marco l'opcio utilitzar GRUP password i encriptar
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image6.png){width="3.8541666666666665in"
> height="3.0305555555555554in"}
>
> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image9.png){width="12.354166666666666in"
> height="8.790062335958005in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic
>
> Aqui fico les particions
>
> Fico la ip estatica
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image8.png){width="5.386111111111111in"
> height="3.4680555555555554in"}
>
> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image11.png){width="12.354166666666666in"
> height="8.021847112860893in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic
>
> Creo l'usuari oriol
>
> Fico el color 24 i la resolucio 1280x1024
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image10.png){width="5.916666666666667in"
> height="2.8541655730533684in"}
>
> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image12.png){width="12.354166666666666in"
> height="8.727350174978127in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic
>
> Selecciono Kubuntu Desktop
>
> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image15.png){width="12.354166666666666in"
> height="9.218591426071741in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic

+-----------------------------------+-----------------------------------+
| d\.                               | > Guarda l'arxiu ks.cfg a         |
|                                   | > l'escritori mateix              |
+===================================+===================================+
+-----------------------------------+-----------------------------------+

> Guardo l'arxiu ks.cfg a l'escritori
>
> Li dono tots el permisos per a poder modificar-ho
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image13.png){width="5.041666666666667in"
> height="0.5416666666666666in"}
>
> e\. Obre la .iso alternate o server amb l'isomaster i posa a l'arrel
> l'arxiu ks.cfg

![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image14.png){width="7.270833333333333in"
height="2.25in"}

> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image17.png){width="12.354166666666666in"
> height="8.868451443569553in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic
>
> Agrego el ks.cfg

+-----------------------------------+-----------------------------------+
| f\.                               | > Amb l'isomaster extreu l'arxiu  |
|                                   | > txt.cfg a l'escritori mateix, i |
|                                   | > modifca'l per tal d'afegir una  |
|                                   | > opció                           |
+===================================+===================================+
+-----------------------------------+-----------------------------------+

> més al menú. Copia la primera opció, caniva el nom i afegeix al final
> ks=cdrom:/ks.cfg
>
> Extrec el txt.cfg per a modificar-ho
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image16.png){width="4.323611111111111in"
> height="3.2083333333333335in"}
>
> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image19.png){width="12.354166666666666in"
> height="10.420562117235345in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic
>
> g\. Guarda els canvis
>
> He canivat el menu label i el quiet

+-----------------------------------+-----------------------------------+
| h\.                               | > Posa aquets arxiu modificat     |
|                                   | > dintre la iso, esborrant primer |
|                                   | > l'antic                         |
+===================================+===================================+
+-----------------------------------+-----------------------------------+

> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image18.png){width="4.416666666666667in"
> height="2.9375in"}
>
> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image21.png){width="12.354166666666666in"
> height="9.323110236220472in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic
>
> i\. Guarda la iso\
> Guardo la iso amb el nom OriolDesates

+-----------------------------------+-----------------------------------+
| j\.                               | > Prova que funcioni en una nova  |
|                                   | > màquina virtual                 |
+===================================+===================================+
+-----------------------------------+-----------------------------------+

> 2\. Realitza la instal·lació desatesa amb el pressed d\'un SO Ubuntu.
> El concepte és el mateix, generar un arxiu de resposta, però enlloc
> del kickstart amb el pressed i desprès posar-lo dintre la iso.
>
> a\. Cerca per internet un arxiu preseed.cfg i modifica'l\
> b. Llavors cal que el posis dintre la iso i que modifiquis el txt.cfg
> afegint una nova opció per a que l'agafi\
> Extrec el cfg
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image20.png){width="4.6875in"
> height="3.1569444444444446in"}
>
> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image23.png){width="12.354166666666666in"
> height="7.624674103237095in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic
>
> Li dono permisos per a modificar-ho
>
> Canvio el append
>
> Elimino el cfg antic i fico el nou modificat
>
> ![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image22.png){width="5.833333333333333in"
> height="4.030555555555556in"}
>
> Administració de SistemesInformàtics en la Xarxa\
> Desenvolupamentd'Aplicacions
> Multiplataforma![](vertopal_11b8fa2ed02f47efad02c1c8049b0610/media/image24.png){width="12.354166666666666in"
> height="5.821718066491688in"}
>
> **M1** -- Implantació de SistemesOperatius\
> **UF3** -- Implantació de ProgramariEspecífic
>
> Guardo la nova iso amb el nom OriolDesatesa2

+-----------------------------------+-----------------------------------+
| c\.                               | > Prova la iso en una nova        |
|                                   | > màquina virtual                 |
+===================================+===================================+
+-----------------------------------+-----------------------------------+
