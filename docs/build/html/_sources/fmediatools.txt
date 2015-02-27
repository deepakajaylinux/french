============
Media Tools
============


synopsis
------------

Ce module vise à installer GC recommandée Media Tool que VLC Media Player qui améliore la productivité du système de l'utilisateur. VLC media player supporte de nombreuses méthodes de compression audio et vidéo et les formats de fichiers, y compris les DVD-Vidéo, CD et protocoles de streaming vidéo. VLC media player (communément appelé VLC) est un appareil portable, libre et open-source, un lecteur multimédia multi-plateforme et serveur de streaming des médias écrits par le projet VideoLAN. Voyons comment ce module aide les installer VLC.

Commande Aide
--------------------

La commande help conduit les utilisateurs concernant l'objet et ainsi que sur les options qui sont inclus dans le module d'outils médiatiques. Les listes de commandes de l'aide sur les autres paramètres d'outils de médias. Il décrit également la syntaxe pour installer VLC. La commande d'aide pour le module d'outils de médias est représentée ci-dessous.

.. code-block:: bash
  
 ptconfigure mediatools help

La syntaxe pour déclarer la commande d'aide ne est pas sensible à la casse qui est un avantage supplémentaire. La capture d'écran ci-dessous vous visualiser sur la commande d'aide en vertu outils de médias.

.. code-block:: bash


	Kevell@corp:/# ptconfigure MediaTools help
	******************************


	This command allows you to install a few GC recommended Media Tools
        for productivity in your system. Currently, we're only including
        VLC Media Player

         MediaTools, media-tools, mediatools, mediatools, media-tools

        - install
        Installs some media tools
        example: ptconfigure mediatools install

	------------------------------
	End Help


installation
---------------


La commande suivante permet d'installer les outils de médias.

.. code-block:: bash

	ptconfigure mediatools install


Visualiser sa fonction La capture d'écran.

.. code-block:: bash


        - install
        Installs some media tools
        example: ptconfigure mediatools install

        ------------------------------
        End Help

Si l'utilisateur procède le processus d'installation, le processus suivant se produit lors de l'installation.

* Extrait des modèles de colis
* Lit listes de paquets.
* Construit arbre de dépendance.
* Lit les informations d'état.
* Répertorie les paquets qui sont automatiquement installés.
* Répertorie les paquets supplémentaires qui sont installés.
* Répertorie les paquets suggérés.
* Répertorie les nouveaux paquets qui sont installés.
* Enfin, les rapports sont clairement affichées avec l'état et les résultats.
* La capture d'écran ci-dessous explique le processus mentionné ci-dessus imagée.

.. code-block:: bash

	Kevell@corp:/# ptconfigure mediatools install
	Install Media Tools? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*         Media Tools!        *
	*******************************
	Extracting templates from packages: 100%
	Reading	package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
  liba52-0.7.4 libaacs0 libass4 libavcodec54 libavformat54 libavutil52
  libbasicusageenvironment0 libbluray1 libcddb2 libchromaprint0 libcrystalhd3
  libdc1394-22 libdca0 libdirac-encoder0 libdirectfb-1.2-9 libdvbpsi8
  libdvdnav4 libdvdread4 libebml4 libenca0 libfaad2 libgnutls28 libgroupsock1
  libgsm1 libhogweed2 libiso9660-8 libkate1 liblivemedia23 libmad0
  libmatroska6 libmodplug1 libmp3lame0 libmpcdec6 libmpeg2-4 libopenjpeg2
  libopus0 libpostproc52 libproxy-tools libresid-builder0c2a
  libschroedinger-1.0-0 libsdl-image1.2 libsdl1.2debian libsidplay2 libssh2-1
  libswscale2 libtar0 libts-0.0-0 libtwolame0 libupnp6 libusageenvironment1
  libva-x11-1 libva1 libvcdinfo0 libvlc5 libvlccore7 libx264-142
  libxcb-composite0 libxcb-xv0 libxvidcore4 libzvbi-common libzvbi0 tsconf
  vlc-data vlc-nox vlc-plugin-notify vlc-plugin-pulse
	Suggested packages:
  libbluray-bdj libchromaprint-tools python-acoustid firmware-crystalhd
  libdvdcss2 debhelper gnutls-bin opus-tools videolan-doc
	The following NEW packages will be installed:
  liba52-0.7.4 libaacs0 libass4 libavcodec54 libavformat54 libavutil52
  libbasicusageenvironment0 libbluray1 libcddb2 libchromaprint0 libcrystalhd3
  libdc1394-22 libdca0 libdirac-encoder0 libdirectfb-1.2-9 libdvbpsi8
  libdvdnav4 libdvdread4 libebml4 libenca0 libfaad2 libgnutls28 libgroupsock1
  libgsm1 libhogweed2 libiso9660-8 libkate1 liblivemedia23 libmad0
  libmatroska6 libmodplug1 libmp3lame0 libmpcdec6 libmpeg2-4 libopenjpeg2
  libopus0 libpostproc52 libproxy-tools libresid-builder0c2a
  libschroedinger-1.0-0 libsdl-image1.2 libsdl1.2debian libsidplay2 libssh2-1
  libswscale2 libtar0 libts-0.0-0 libtwolame0 libupnp6 libusageenvironment1
  libva-x11-1 libva1 libvcdinfo0 libvlc5 libvlccore7 libx264-142
 libxcb-composite0 libxcb-xv0 libxvidcore4 libzvbi-common libzvbi0 tsconf vlc
  vlc-data vlc-nox vlc-plugin-notify vlc-plugin-pulse
	0 upgraded, 67 newly installed, 0 to remove and 6 not upgraded.
	Need to get 17.7 MB of archives.
	After this operation, 72.9 MB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libaacs0 amd64 0.7.0-1 [47.3 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe libavutil52 amd64 6:9.16-0ubuntu0.14.04.1 [67.2 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libgsm1 amd64 1.0.13-4 [27.1 kB]
	Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmp3lame0 amd64 3.99.5+repack1-3ubuntu1 [158 kB]
	Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libopenjpeg2 amd64 1.3+dfsg-4.7ubuntu1 [64.3 kB]
	Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty/main libopus0 amd64 1.1-0ubuntu1 [153 kB]
	Get:7 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libschroedinger-1.0-0 amd64 1.0.11-2ubuntu1 [268 kB]
	Get:8 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libva1 amd64 1.3.0-2 [38.6 kB]
	Get:9 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libx264-142 amd64 2:0.142.2389+git956c8d8-2 [575 kB]
	Get:10 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libxvidcore4 amd64 2:1.3.2-9ubuntu1 [298 kB]
	Get:11 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe libavcodec54 amd64 6:9.16-0ubuntu0.14.04.1 [2,348 kB]
	Get:12 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe libavformat54 amd64 6:9.16-0ubuntu0.14.04.1 [481 kB]
	Get:13 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libbasicusageenvironment0 amd64 2014.01.13-1 [16.4 kB]
	Get:14 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libbluray1 amd64 1:0.5.0-1 [98.9 kB]
	Get:15 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libcrystalhd3 amd64 1:0.0~git20110715.fdd2f19-9ubuntu1 [52.7 kB]
	Get:16 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libdirac-encoder0 amd64 1.0.2-6ubuntu1 [243 kB]
	Get:17 http://in.archive.ubuntu.com/ubuntu/ trusty/universe tsconf all 1.0-12 [6,990 B]
	Get:18 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libts-0.0-0 amd64 1.0-12 [18.8 kB]
	Get:19 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libdirectfb-1.2-9 amd64 1.2.10.0-5 [759 kB]
	Get:20 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libdvbpsi8 amd64 1.0.0-3 [52.3 kB]
	Get:21 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libdvdread4 amd64 4.2.1-2ubuntu1 [50.2 kB]
	Get:22 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libdvdnav4 amd64 4.2.1-3 [42.4 kB]
	Get:23 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libebml4 amd64 1.3.0-2 [51.7 kB]
	Get:24 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libenca0 amd64 1.15-2 [53.7 kB]
	Get:25 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libfaad2 amd64 2.7-8 [176 kB]
	Get:26 http://in.archive.ubuntu.com/ubuntu/ trusty/main libhogweed2 amd64 2.7.1-1 [133 kB]
	Get:27 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libgnutls28 amd64 3.2.11-2ubuntu1 [539 kB]
	Get:28 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libgroupsock1 amd64 2014.01.13-1 [22.0 kB]
	Get:29 http://in.archive.ubuntu.com/ubuntu/ trusty/universe liblivemedia23 amd64 2014.01.13-1 [267 kB]
	Get:30 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmad0 amd64 0.15.1b-8ubuntu1 [71.5 kB]
	Get:31 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmatroska6 amd64 1.4.1-2 [155 kB]
	Get:32 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmpeg2-4 amd64 0.5.1-5ubuntu1 [56.4 kB]
	Get:33 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libsdl1.2debian amd64 1.2.15-8ubuntu1.1 [162 kB]
	Get:34 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libsdl-image1.2 amd64 1.2.12-5build2 [28.2 kB]
	Get:35 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libssh2-1 amd64 1.4.3-2 [66.3 kB]
	Get:36 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe libswscale2 amd64 6:9.16-0ubuntu0.14.04.1 [81.6 kB]
	Get:37 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libusageenvironment1 amd64 2014.01.13-1 [7,510 B]
	Get:38 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libva-x11-1 amd64 1.3.0-2 [11.7 kB]
	Get:39 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libproxy-tools amd64 0.4.11-0ubuntu4 [5,258 B]
	Get:40 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe vlc-data all 2.1.4-0ubuntu14.04.1 [4,886 kB]
	Get:41 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe libvlccore7 amd64 2.1.4-0ubuntu14.04.1 [342 kB]
	Get:42 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe libvlc5 amd64 2.1.4-0ubuntu14.04.1 [39.9 kB]
	Get:43 http://in.archive.ubuntu.com/ubuntu/ trusty/main libxcb-composite0 amd64 1.10-2ubuntu1 [5,036 B]
	Get:44 http://in.archive.ubuntu.com/ubuntu/ trusty/main libxcb-xv0 amd64 1.10-2ubuntu1 [8,772 B]
	Get:45 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libzvbi-common all 0.2.35-2 [38.7 kB]
	Get:46 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libzvbi0 amd64 0.2.35-2 [293 kB]
	Get:47 http://in.archive.ubuntu.com/ubuntu/ trusty/universe liba52-0.7.4 amd64 0.7.4-17 [32.1 kB]
	Get:48 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libass4 amd64 0.10.1-3ubuntu1 [47.2 kB]
	Get:49 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libcddb2 amd64 1.3.2-4fakesync2 [33.9 kB]
	Get:50 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libchromaprint0 amd64 1.1-1 [33.1 kB]
	Get:51 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libdc1394-22 amd64 2.2.1-2ubuntu2 [75.0 kB]
	Get:52 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libdca0 amd64 0.0.5-6ubuntu1 [93.5 kB]
	Get:53 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libkate1 amd64 0.4.1-1ubuntu1 [37.3 kB]
	Get:54 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmodplug1 amd64 1:0.8.8.4-4.1 [147 kB]
	Get:55 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmpcdec6 amd64 2:0.1~r459-1ubuntu3 [30.7 kB]
	Get:56 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libpostproc52 amd64 6:0.git20120821-4 [30.6 kB]
	Get:57 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libresid-builder0c2a amd64 2.1.1-14 [39.4 kB]
	Get:58 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libsidplay2 amd64 2.1.1-14 [102 kB]
	Get:59 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libtwolame0 amd64 0.3.13-1ubuntu1 [48.8 kB]
	Get:60 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libupnp6 amd64 1:1.6.17-1.2 [142 kB]
	Get:61 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libiso9660-8 amd64 0.83-4.1ubuntu1 [18.8 kB]
	Get:62 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libvcdinfo0 amd64 0.7.24+dfsg-0.1ubuntu2 [89.5 kB]
	Get:63 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe vlc-nox amd64 2.1.4-0ubuntu14.04.1 [2,033 kB]
	Get:64 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe libtar0 amd64 1.2.20-3ubuntu0.1 [18.2 kB]
	Get:65 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe vlc amd64 2.1.4-0ubuntu14.04.1 [1,213 kB]
	Get:66 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe vlc-plugin-notify amd64 2.1.4-0ubuntu14.04.1 [5,262 B]
	Get:67 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe vlc-plugin-pulse amd64 2.1.4-0ubuntu14.04.1 [16.7 kB]
	Fetched 17.7 MB in 1min 4s (274 kB/s)
	Preparing to unpack .../libupnp6_1%3a1.6.17-1.2_amd64.deb ...
	Unpacking libupnp6 (1:1.6.17-1.2) ...
	Selecting previously unselected package libiso9660-8.
	Preparing to unpack .../libiso9660-8_0.83-4.1ubuntu1_amd64.deb ...
	Unpacking libiso9660-8 (0.83-4.1ubuntu1) ...
	Selecting previously unselected package libvcdinfo0.
	Preparing to unpack .../libvcdinfo0_0.7.24+dfsg-0.1ubuntu2_amd64.deb ...
	Unpacking libvcdinfo0 (0.7.24+dfsg-0.1ubuntu2) ...
	Selecting previously unselected package vlc-nox.
	Preparing to unpack .../vlc-nox_2.1.4-0ubuntu14.04.1_amd64.deb ...
	Unpacking vlc-nox (2.1.4-0ubuntu14.04.1) ...
	Selecting previously unselected package libtar0.
	Preparing to unpack .../libtar0_1.2.20-3ubuntu0.1_amd64.deb ...
	Unpacking libtar0 (1.2.20-3ubuntu0.1) ...
	Selecting previously unselected package vlc.
	Preparing to unpack .../vlc_2.1.4-0ubuntu14.04.1_amd64.deb ...
	Unpacking vlc (2.1.4-0ubuntu14.04.1) ...
	Selecting previously unselected package vlc-plugin-notify.
	Preparing to unpack .../vlc-plugin-notify_2.1.4-0ubuntu14.04.1_amd64.deb ...
	Unpacking vlc-plugin-notify (2.1.4-0ubuntu14.04.1) ...
	Selecting previously unselected package vlc-plugin-pulse.
	Preparing to unpack .../vlc-plugin-pulse_2.1.4-0ubuntu14.04.1_amd64.deb ...
	Unpacking vlc-plugin-pulse (2.1.4-0ubuntu14.04.1) ...
	Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
	Processing triggers for hicolor-icon-theme (0.13-1) ...
	Processing triggers for mime-support (3.54ubuntu1.1) ...
	Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
	Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
	Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
	Rebuilding /usr/share/applications/bamf-2.index...
	Setting up libaacs0:amd64 (0.7.0-1) ...
	Setting up libavutil52:amd64 (6:9.16-0ubuntu0.14.04.1) ...
	Setting up libgsm1:amd64 (1.0.13-4) ...
	Setting up libmp3lame0:amd64 (3.99.5+repack1-3ubuntu1) ...
	Setting up libopenjpeg2:amd64 (1.3+dfsg-4.7ubuntu1) ...
	Setting up libopus0 (1.1-0ubuntu1) ...
	Setting up libschroedinger-1.0-0:amd64 (1.0.11-2ubuntu1) ...
	Setting up libva1:amd64 (1.3.0-2) ...
	Setting up libx264-142:amd64 (2:0.142.2389+git956c8d8-2) ...
	Setting up libxvidcore4:amd64 (2:1.3.2-9ubuntu1) ...
	Setting up libavcodec54:amd64 (6:9.16-0ubuntu0.14.04.1) ...
	Setting up libavformat54:amd64 (6:9.16-0ubuntu0.14.04.1) ...
	Setting up libbasicusageenvironment0 (2014.01.13-1) ...
	Setting up libbluray1:amd64 (1:0.5.0-1) ...
	Setting up libcrystalhd3:amd64 (1:0.0~git20110715.fdd2f19-9ubuntu1) ...
	Setting up libdirac-encoder0:amd64 (1.0.2-6ubuntu1) ...
	Setting up tsconf (1.0-12) ...
	Setting up libts-0.0-0:amd64 (1.0-12) ...
	Setting up libdirectfb-1.2-9:amd64 (1.2.10.0-5) ...
	Setting up libdvbpsi8:amd64 (1.0.0-3) ...
	Setting up libdvdread4:amd64 (4.2.1-2ubuntu1) ...
	Setting up libdvdnav4:amd64 (4.2.1-3) ...
	Setting up libebml4:amd64 (1.3.0-2) ...
	Setting up libenca0:amd64 (1.15-2) ...
	Setting up libfaad2:amd64 (2.7-8) ...
	Setting up libhogweed2:amd64 (2.7.1-1) ...
	Setting up libgnutls28:amd64 (3.2.11-2ubuntu1) ...
	Setting up libgroupsock1 (2014.01.13-1) ...
	Setting up liblivemedia23 (2014.01.13-1) ...
	Setting up libmad0:amd64 (0.15.1b-8ubuntu1) ...
	Setting up libmatroska6:amd64 (1.4.1-2) ...
	Setting up libmpeg2-4:amd64 (0.5.1-5ubuntu1) ...
	Setting up libsdl1.2debian:amd64 (1.2.15-8ubuntu1.1) ...
	Setting up libsdl-image1.2:amd64 (1.2.12-5build2) ...
	Setting up libssh2-1:amd64 (1.4.3-2) ...
	Setting up libswscale2:amd64 (6:9.16-0ubuntu0.14.04.1) ...
	Setting up libusageenvironment1 (2014.01.13-1) ...
	Setting up libva-x11-1:amd64 (1.3.0-2) ...
	Setting up libproxy-tools (0.4.11-0ubuntu4) ...
	Setting up vlc-data (2.1.4-0ubuntu14.04.1) ...
	Setting up libvlccore7 (2.1.4-0ubuntu14.04.1) ...
	Setting up libvlc5 (2.1.4-0ubuntu14.04.1) ...
	Setting up libxcb-composite0:amd64 (1.10-2ubuntu1) ...
	Setting up libxcb-xv0:amd64 (1.10-2ubuntu1) ...
	Setting up libzvbi-common (0.2.35-2) ...
	Setting up libzvbi0:amd64 (0.2.35-2) ...
	Setting up liba52-0.7.4 (0.7.4-17) ...
	Setting up libass4:amd64 (0.10.1-3ubuntu1) ...
	Setting up libcddb2 (1.3.2-4fakesync2) ...
	Setting up libchromaprint0:amd64 (1.1-1) ...
	Setting up libdc1394-22:amd64 (2.2.1-2ubuntu2) ...
	Setting up libdca0:amd64 (0.0.5-6ubuntu1) ...
	Setting up libkate1 (0.4.1-1ubuntu1) ...
	Setting up libmodplug1 (1:0.8.8.4-4.1) ...
	Setting up libmpcdec6 (2:0.1~r459-1ubuntu3) ...
	Setting up libpostproc52 (6:0.git20120821-4) ...
	Setting up libresid-builder0c2a (2.1.1-14) ...
	Setting up libsidplay2 (2.1.1-14) ...
	Setting up libtwolame0 (0.3.13-1ubuntu1) ...
	Setting up libupnp6 (1:1.6.17-1.2) ...
	Setting up libiso9660-8 (0.83-4.1ubuntu1) ...
	Setting up libvcdinfo0 (0.7.24+dfsg-0.1ubuntu2) ...
	Setting	up vlc-nox (2.1.4-0ubuntu14.04.1) ...
	Setting up libtar0 (1.2.20-3ubuntu0.1) ...
	Setting up vlc (2.1.4-0ubuntu14.04.1) ...
	Setting up vlc-plugin-notify (2.1.4-0ubuntu14.04.1) ...
	Setting up vlc-plugin-pulse (2.1.4-0ubuntu14.04.1) ...
		Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
	[Pharaoh Logging] Adding Package vlc from the Packager Apt executed correctly
	Reading package lists...
	Building dependency tree...
	Reading state information...
	libdvdread4 is already the newest version.
	libdvdread4 set to manually installed.
	0 upgraded, 0 newly installed, 0 to remove and 6 not upgraded.
	[Pharaoh Logging] Package libdvdread4 from the Packager Apt is already installed, so not installing.
	Creating /tmp/ptconfigure-temp-script-86836778897.sh
	chmod 755 /tmp/ptconfigure-temp-script-86836778897.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-86836778897.sh Permissions
	Executing /tmp/ptconfigure-temp-script-86836778897.sh
	--2015-01-10 01:11:57--  http://download.videolan.org/pub/debian/stable//Packages
	Resolving download.videolan.org (download.videolan.org)... 195.154.216.18
	Connecting to download.videolan.org (download.videolan.org)|195.154.216.18|:80... connected.
	HTTP request sent, awaiting response... 200 OK
	Length: 3520 (3.4K) [application/octet-stream]
	Saving to: ‘/tmp/dvdcss-vaA1iO/Packages’
	
		100%[=====================================================================================================>] 3,520       --.-K/s   in 0.007s  
	
	2015-01-10 01:11:59 (523 KB/s) - ‘/tmp/dvdcss-vaA1iO/Packages’ saved [3520/3520]
	
	--2015-01-10 01:11:59--  http://download.videolan.org/pub/debian/stable/stable/libdvdcss2_1.2.13-0_amd64.deb
	Resolving download.videolan.org (download.videolan.org)... 195.154.216.18
	Connecting to download.videolan.org (download.videolan.org)|195.154.216.18|:80... connected.
	HTTP request sent, awaiting response... 200 OK
	Length: 44462 (43K) [application/octet-stream]
	Saving to: ‘/tmp/dvdcss-vaA1iO/libdvdcss.deb’
	
	100%[=====================================================================================================>] 44,462       118KB/s   in 0.4s   
	
	2015-01-10 01:12:00 (118 KB/s) - ‘/tmp/dvdcss-vaA1iO/libdvdcss.deb’ saved [44462/44462]
	
	Selecting previously unselected package libdvdcss2.
	(Reading database ... 202893 files and directories currently installed.)
	Preparing to unpack .../dvdcss-vaA1iO/libdvdcss.deb ...
	Unpacking libdvdcss2 (1.2.13-0) ...
	Setting up libdvdcss2 (1.2.13-0) ...
	Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
	Temp File /tmp/ptconfigure-temp-script-86836778897.sh Removed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	MediaTools: Success
	------------------------------
	Installer Finished
	******************************


Options
----------


.. cssclass:: table-bordered

 +----------------------+-----------------------------------------------+-------------+--------------------------------------------+
 | paramètres           | paramètre alternatif                          | option      | commentaires                               |
 +======================+===============================================+=============+============================================+
 |Install Media Tools?  | au lieu de Media Tools, , les solutions       | Y(Yes)      | Si l'utilisateur souhaite procéder le      |
 |(Y/N)                 | suivantes peuvent également être utilisés     |             | processus d'installation qu'ils peuvent    |
 |                      | MediaTools, media-tools, mediatools.          |             | entrée comme Y                             |
 +----------------------+-----------------------------------------------+-------------+--------------------------------------------+
 |Install Media Tools?  | au lieu de Media Tools, , les solutions       | N(No)       | Si l'utilisateur souhaite quitter le       |
 |(Y/N)                 | suivantes peuvent également être utilisés     |             | processus d'installation qu'ils peuvent    |
 |                      | MediaTools, media-tools, mediatools.          |             | entrée comme N.|                           |
 +----------------------+-----------------------------------------------+-------------+--------------------------------------------+
 
   
avantages
------------


* Les paramètres utilisés dans les opérations d'aide et d'installation ne sont pas sensibles à la casse qui est un avantage supplémentaire en 
  rapport aux autres.
* Utilisation de ce module de la productivité du système peut être améliorée.
* Il est bien de choses à faire dans les deux Ubuntu et ainsi que Cent OS.
* Ce module facilite l'installation GC recommandée outils médiatiques.
