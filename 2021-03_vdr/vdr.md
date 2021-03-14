# VDR Fedora et al

https://src.fedoraproject.org/rpms/vdr
https://src.fedoraproject.org/rpms/vdr/blob/rawhide/f/vdr.spec

## Repos

http://git.tvdr.de/vdr.git
https://bitbucket.org/powARman/dvbhddevice/src/master/

https://github.com/rofafor/vdr-plugin-satip
https://github.com/gentoo/gentoo/pull/18919

## Patches Fedora

	
Source0:        ftp://ftp.tvdr.de/vdr/%{name}-%{version}.tar.bz2
Source1:        %{name}.service
Source2:        %{name}.sysconfig
Source3:        %{name}.sudoers
Source5:        %{name}-reccmds.conf
Source6:        %{name}-commands.conf
Source7:        %{name}-runvdr.sh
Source8:        %{name}-dvbsddevice.conf
Source9:        %{name}-config.sh
Source10:       %{name}-README.package
Source11:       %{name}-skincurses.conf
Source12:       %{name}-dvbhddevice.conf
Source13:       %{name}-timercmds.conf
Source14:       %{name}-shutdown.sh
Source15:       %{name}-moveto.sh
Source16:       %{name}-CHANGES.package.old
Source17:       %{name}.macros
Source18:       http://cdn.debian.net/debian/pool/main/v/vdr/vdr_2.2.0-5.debian.tar.bz2
Source19:       %{name}-check-setup.sh
Source20:       %{name}-rcu.conf
Source21:       %{name}-set-wakeup.sh
Source30:       https://bitbucket.org/powARman/dvbhddevice/get/2ea854ae8c7a.zip
Source31:       ftp://ftp.tvdr.de/vdr/Plugins/vdr-dvbsddevice-2.2.0.tgz
Source32:       ftp://ftp.tvdr.de/vdr/Plugins/vdr-rcu-2.2.0.tgz
 
Patch0:         define_AUDIO_GET_PTS.patch
Patch1:         http://zap.tartarus.org/~ds/debian/dists/stable/main/source/vdr_1.4.5-2.ds.diff.gz
Patch2:         http://www.saunalahti.fi/~rahrenbe/vdr/patches/vdr-2.4.6-editrecording.patch.gz
# Extracted from http://copperhead.htpc-forum.de/downloads/extensionpatch/extpngvdr1.7.21v1.diff.gz
Patch3:         %{name}-1.7.21-plugin-missing.patch
Patch4:         %{name}-2.4.0-paths.patch
# http://vdrportal.de/board/thread.php?postid=343665#post343665
Patch7:         12_osdbase-maxitems.patch
Patch8:         http://www.saunalahti.fi/~rahrenbe/vdr/patches/vdr-2.4.6-lcn-support-v2.patch.gz
# http://www.udo-richter.de/vdr/naludump.en.html
Patch10:        http://www.udo-richter.de/vdr/files/vdr-2.1.5-naludump-0.1.diff
# http://article.gmane.org/gmane.linux.vdr/43590
Patch11:        %{name}-2.4.0-mainmenuhooks101.patch
# Sent upstream 2016-06-17
Patch15:        %{name}-1.7.37-fedora-pkgconfig.patch
# https://gitlab.com/pbiering/extrecmenung/-/blob/adjust-EPG-rename-title-shorttext/contrib/vdr-2.4.4-RecordingInfo.patch
Patch16:         vdr-2.4.4-RecordingInfo.patch
# https://www.vdr-portal.de/index.php?attachment/44831-vdr-2-4-6-clearobsoletechannels-diff/
Patch99:        %{name}-2.4.6-ClearObsoleteChannels2.diff

## Patches Gentoo

mainmenuhooks? ( http://vdr.websitec.de/download/${PN}/${PN}-2.4.1/${PN}-2.4.1_mainmenuhook-1.0.1.patch.bz2 )
	menuorg? ( https://projects.vdr-developer.org/projects/plg-menuorg/repository/revisions/master/raw/vdr-patch/vdr-menuorg-2.3.x.diff )
	naludump? ( http://www.udo-richter.de/vdr/files/vdr-2.1.5-naludump-0.1.diff )
	pinplugin? ( http://vdr.websitec.de/download/${PN}/${P}/${P}_pinplugin.patch.bz2 )
	ttxtsubs? ( http://vdr.websitec.de/download/${PN}/${P}/${P}_ttxtsubs_v2.patch.bz2 )
	permashift? ( http://vdr.websitec.de/download/${PN}/${P}/vdr-2.4-patch-for-permashift.diff.bz2 )"
 

