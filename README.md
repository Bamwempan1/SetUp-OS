# SetUp-OS
 Fichier et ligne de commande pour restart un windows et linux proprement avec un ASUS g551jm

## A Faire
- [ ] Mettre les lignes de commande dans le ReadMe
- [ ] Ecrire un readme Proprement !

### Ordi
[Spéc ordi](https://forum.hardware.fr/hfr/OrdinateursPortables/portable/unique-asus-g551-sujet_76648_1.htm)

## Windows

### Instaler cache
[Tutoriel Pour installer cache](https://forum.hardware.fr/hfr/OrdinateursPortables/portable/unique-asus-g551-sujet_76648_17.htm#t1461033)

### Vérifier si le cache est en marche
<pre>
  eccmd.exe -info
</pre>

### Logiciel

- [ZHP Cleaner](https://www.nicolascoolman.com/fr/download/zhpcleaner/?wpdmdl=5411&refresh=5cf00abfc21561559235263)
- [Autorun](https://anga.tv/logiciels/AutoRuns/autoruns.exe)

### Si problème Horloge Windows/Linux

[Si le .reg ne fonctionne pas](https://lifehacker.com/fix-incorrect-clock-settings-in-windows-when-dual-booti-5742148)

<pre>Lancer TimeUniversal.reg</pre>

### Si le clavier ne s'allume pas
<pre>Lancer le pilote ATKpackage</pre>

## Linux

### Armoniser Windows et Linux
[Tuto Armoniser Window et Linux](https://www.howtogeek.com/howto/35807/how-to-harmonize-your-dual-boot-setup-for-windows-and-ubuntu/)

### Monter partition au démarage
[Tuto Partition](https://doc.ubuntu-fr.org/gnome-disk-utility#monter_une_partition_automatiquement_au_demarrage)

### Régler Ethernet
[Tuto Ethernet](https://unixblogger.com/how-to-get-your-realtek-rtl8111rtl8168-working-updated-guide/)
<pre>
sudo apt-get install build-essential linux-headers-$(uname -r)
</pre>
[Suite tuto](https://www.realtek.com/en/component/zoo/category/network-interface-controllers-10-100-1000m-gigabit-ethernet-pci-express-software)

Blaclist le driver de base
<pre>
sudo sh -c 'echo blacklist r8169 >> /etc/modprobe.d/blacklist.conf'

Install

sudo ./autorun.sh

Reboot
</pre>

### Faire des racourcies pour les dossiers Windows sur le dossier Home linux
<pre>
ln -s /mnt/09044826333377E0/Vidéos  /home/kevin
</pre>

Si les dossier ne sont accessible que en lecture utiliser la commande suivante sur le disque utile
<pre>
sudo ntfsfix /dev/sda6
</pre>

### NUMIX THEME ICON