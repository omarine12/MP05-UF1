Administració de SistemesInformàtics en la Xarxa![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.001.png)

Desenvolupamentd’Aplicacions Multiplataforma

**M1** – Implantació de SistemesOperatius

**UF3** – Implantació de ProgramariEspecífic


**Instal·lació desatesa amb fitxer de resposta**

Per a fer una instal·lació desatesa amb Ubuntu existeixen dues opcions, la primera és fer-ho amb el kickstart, la qual té l’avantatja que és més senzilla d’utilitzar, però és menys completa. L’altra és amb el preseed, és més complexa, però la configuració és molt més extensa.

<a name="_heading=h.gjdgxs"></a>Recursos necessaris:

- Màquina base amfitrió Ubuntu 14.04, Ubuntu 16.04...
- Alguna .iso versió alternate o server **DINTRE** de la MV amfitrió
- Instal·lació del isomaster

Utilitzo la seguent comanda

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.002.png)

**\*\*\* Enlloc de l’isomaster es pot fer ús de rsync per a extreure tot lo de la iso i desprès mkisofs per a tornar a generar-la**

1. Realitza la instal·lació desatesa amb el kickstart d'un SO Ubuntu
   1. Actualitza repositoris

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.003.png)

1. Instal·la system-config-kickstart

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.004.png)



1. Obre amb system-config-kickstart i configura els paràmetre que creguis necessaris

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.005.png)


He modificat el idioma default a catala, el teclat a l’español i la hora

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.006.png)

d

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.007.png)



f

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.008.png)

d

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.009.png)



d

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.010.png)

d

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.011.png)

d

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.012.png)





1. Guarda l’arxiu ks.cfg a l’escritori mateix

Guardo l’arxiu ks.cfg a l’escritori

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.013.png)

Li dono tots el permisos per a poder modificar-ho

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.014.png)

1. Obre la .iso alternate o server amb l’isomaster i posa a l’arrel l’arxiu ks.cfg

d

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.015.png)



d

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.016.png)

1. Amb l’isomaster extreu l’arxiu txt.cfg a l’escritori mateix, i modifca’l per tal d’afegir una opció més al menú. Copia la primera opció, caniva el nom i afegeix al final ks=cdrom:/ks.cfg

d

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.017.png)



1. Guarda els canvis

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.018.png)

1. Posa aquets arxiu modificat dintre la iso, esborrant primer l’antic

D

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.019.png)



1. Guarda la iso

Guardo la iso amb el nom OriolDesates

![](Aspose.Words.d2de289b-565c-406b-b7a9-d6f8e9990cc5.020.png)

1. Prova que funcioni en una nova màquina virtual
1. Realitza la instal·lació desatesa amb el pressed d'un SO Ubuntu. El concepte és el mateix, generar un arxiu de resposta, però enlloc del kickstart amb el pressed i desprès posar-lo dintre la iso.
   1. Cerca per internet un arxiu preseed.cfg i modifica’l
   1. Llavors cal que el posis dintre la iso i que modifiquis el txt.cfg afegint una nova opció per a que l’agafi
   1. Prova la iso en una nova màquina virtual


