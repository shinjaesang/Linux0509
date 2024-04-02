root@shinjaesang-virtual-machine:~# yes > /dev/null
kill
^Z                                                          
[1]+  멈춤                  yes > /dev/null
root@shinjaesang-virtual-machine:~# bg
[1]+ yes > /dev/null &
root@shinjaesang-virtual-machine:~# jobs
[1]+  실행중               yes > /dev/null &
root@shinjaesang-virtual-machine:~# fg 1
yes > /dev/null
^C
root@shinjaesang-virtual-machine:~# ^C
root@shinjaesang-virtual-machine:~# nano
root@shinjaesang-virtual-machine:~# nano &
[1] 2883
root@shinjaesang-virtual-machine:~# ^C

[1]+  멈춤                  nano
root@shinjaesang-virtual-machine:~# nano &
[2] 2884
root@shinjaesang-virtual-machine:~# fg 1
nano

[2]-  멈춤                  nano
root@shinjaesang-virtual-machine:~# fg 2
nano
root@shinjaesang-virtual-machine:~# 


root@shinjaesang-virtual-machine:~# cd /lib/systemd/system
root@shinjaesang-virtual-machine:/lib/systemd/system# ls *.service
ModemManager.service                    rescue.service
NetworkManager-dispatcher.service       rsync.service
NetworkManager-wait-online.service      rsyslog.service
NetworkManager.service                  rtkit-daemon.service
accounts-daemon.service                 saned.service
acpid.service                           saned@.service
alsa-restore.service                    secureboot-db.service
alsa-state.service                      serial-getty@.service
alsa-utils.service                      setvtrgb.service
anacron.service                         snapd.aa-prompt-listener.service
apparmor.service                        snapd.apparmor.service
apport-autoreport.service               snapd.autoimport.service
apport-forward@.service                 snapd.core-fixup.service
apt-daily-upgrade.service               snapd.failure.service
apt-daily.service                       snapd.recovery-chooser-trigger.service
apt-news.service                        snapd.seeded.service
autovt@.service                         snapd.service
avahi-daemon.service                    snapd.snap-repair.service
bluetooth.service                       snapd.system-shutdown.service
bolt.service                            speech-dispatcherd.service
brltty-udev.service                     spice-vdagent.service
brltty.service                          spice-vdagentd.service
colord.service                          switcheroo-control.service
configure-printer@.service              system-update-cleanup.service
console-getty.service                   systemd-ask-password-console.service
console-setup.service                   systemd-ask-password-plymouth.service
container-getty@.service                systemd-ask-password-wall.service
cron.service                            systemd-backlight@.service
cryptdisks-early.service                systemd-binfmt.service
cryptdisks.service                      systemd-bless-boot.service
cups-browsed.service                    systemd-boot-check-no-failures.service
cups.service                            systemd-boot-system-token.service
dbus-org.freedesktop.hostname1.service  systemd-exit.service
dbus-org.freedesktop.locale1.service    systemd-fsck-root.service
dbus-org.freedesktop.login1.service     systemd-fsck@.service
dbus-org.freedesktop.timedate1.service  systemd-fsckd.service
dbus.service                            systemd-halt.service
debug-shell.service                     systemd-hibernate-resume@.service
dmesg.service                           systemd-hibernate.service
dpkg-db-backup.service                  systemd-hostnamed.service
e2scrub@.service                        systemd-hybrid-sleep.service
e2scrub_all.service                     systemd-initctl.service
e2scrub_fail@.service                   systemd-journal-flush.service
e2scrub_reap.service                    systemd-journald.service
emergency.service                       systemd-journald@.service
esm-cache.service                       systemd-kexec.service
fprintd.service                         systemd-localed.service
friendly-recovery.service               systemd-logind.service
fstrim.service                          systemd-machine-id-commit.service
fwupd-offline-update.service            systemd-modules-load.service
fwupd-refresh.service                   systemd-network-generator.service
fwupd.service                           systemd-networkd-wait-online.service
gdm.service                             systemd-networkd.service
gdm3.service                            systemd-oomd.service
geoclue.service                         systemd-poweroff.service
getty-static.service                    systemd-pstore.service
getty@.service                          systemd-quotacheck.service
gpu-manager.service                     systemd-random-seed.service
grub-common.service                     systemd-reboot.service
grub-initrd-fallback.service            systemd-remount-fs.service
hwclock.service                         systemd-resolved.service
iio-sensor-proxy.service                systemd-rfkill.service
initrd-cleanup.service                  systemd-suspend-then-hibernate.service
initrd-parse-etc.service                systemd-suspend.service
initrd-switch-root.service              systemd-sysctl.service
initrd-udevadm-cleanup-db.service       systemd-sysext.service
ipp-usb.service                         systemd-sysusers.service
irqbalance.service                      systemd-time-wait-sync.service
kerneloops.service                      systemd-timedated.service
keyboard-setup.service                  systemd-timesyncd.service
kmod-static-nodes.service               systemd-tmpfiles-clean.service
kmod.service                            systemd-tmpfiles-setup-dev.service
logrotate.service                       systemd-tmpfiles-setup.service
man-db.service                          systemd-udev-settle.service
modprobe@.service                       systemd-udev-trigger.service
motd-news.service                       systemd-udevd.service
networkd-dispatcher.service             systemd-update-utmp-runlevel.service
nftables.service                        systemd-update-utmp.service
nm-priv-helper.service                  systemd-user-sessions.service
open-vm-tools.service                   systemd-volatile-root.service
openvpn-client@.service                 thermald.service
openvpn-server@.service                 ua-reboot-cmds.service
openvpn.service                         ua-timer.service
openvpn@.service                        ubuntu-advantage-desktop-daemon.service
packagekit-offline-update.service       ubuntu-advantage.service
packagekit.service                      udev.service
plymouth-halt.service                   udisks2.service
plymouth-kexec.service                  ufw.service
plymouth-log.service                    unattended-upgrades.service
plymouth-poweroff.service               update-notifier-download.service
plymouth-quit-wait.service              update-notifier-motd.service
plymouth-quit.service                   upower.service
plymouth-read-write.service             usb_modeswitch@.service
plymouth-reboot.service                 usbmuxd.service
plymouth-start.service                  user-runtime-dir@.service
plymouth-switch-root-initramfs.service  user@.service
plymouth-switch-root.service            uuidd.service
plymouth.service                        vgauth.service
polkit.service                          wacom-inputattach@.service
power-profiles-daemon.service           whoopsie.service
procps.service                          wpa_supplicant-nl80211@.service
pulseaudio-enable-autospawn.service     wpa_supplicant-wired@.service
quotaon.service                         wpa_supplicant.service
rc-local.service                        wpa_supplicant@.service
rc.service                              x11-common.service
rcS.service
root@shinjaesang-virtual-machine:/lib/systemd/system# ls *.socket
acpid.socket            systemd-journald-audit.socket
apport-forward.socket   systemd-journald-dev-log.socket
avahi-daemon.socket     systemd-journald-varlink@.socket
cups.socket             systemd-journald.socket
dbus.socket             systemd-journald@.socket
saned.socket            systemd-networkd.socket
snapd.socket            systemd-rfkill.socket
spice-vdagentd.socket   systemd-udevd-control.socket
syslog.socket           systemd-udevd-kernel.socket
systemd-fsckd.socket    uuidd.socket
systemd-initctl.socket
root@shinjaesang-virtual-machine:/lib/systemd/system# 


root@shinjaesang-virtual-machine:~# cd Downloads
bash: cd: Downloads: 그런 파일이나 디렉터리가 없습니다
root@shinjaesang-virtual-machine:~# cd 다운로드
root@shinjaesang-virtual-machine:~/다운로드# ls
root@shinjaesang-virtual-machine:~/다운로드# wget https;//dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
--2023-05-16 10:24:59--  http://https/
https (https) 해석 중... ^[[A^C
root@shinjaesang-virtual-machine:~/다운로드# wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
--2023-05-16 10:25:35--  https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
dl.google.com (dl.google.com) 해석 중... 216.58.203.78, 2404:6800:4005:814::200e
다음으로 연결 중: dl.google.com (dl.google.com)|216.58.203.78|:443... 연결했습니다.
HTTP 요청을 보냈습니다. 응답 기다리는 중... 200 OK
길이: 94953468 (91M) [application/x-debian-package]
저장 위치: ‘google-chrome-stable_current_amd64.deb’

google-chrome-stabl 100%[===================>]  90.55M  38.3MB/s    / 2.4s     

2023-05-16 10:25:37 (38.3 MB/s) - ‘google-chrome-stable_current_amd64.deb’ 저장함 [94953468/94953468]

root@shinjaesang-virtual-machine:~/다운로드# ls
google-chrome-stable_current_amd64.deb
root@shinjaesang-virtual-machine:~/다운로드# bpkg -i google-chrome-stable-current_amd64.deb
명령어 'bpkg' 을(를) 찾을 수 없습니다. 다음 명령어로 시도하시겠습니까:
  deb dpkgdpkg의 명령어 ' (1.21.1ubuntu2.1)'
Try: apt install <deb name>
root@shinjaesang-virtual-machine:~/다운로드# bpkg -i google-chrome-stable_current_amd64.deb
명령어 'bpkg' 을(를) 찾을 수 없습니다. 다음 명령어로 시도하시겠습니까:
  deb dpkgdpkg의 명령어 ' (1.21.1ubuntu2.1)'
Try: apt install <deb name>
root@shinjaesang-virtual-machine:~/다운로드# apt install ./google-chrome-stable_current_amd64.deb
패키지 목록을 읽는 중입니다... 완료
의존성 트리를 만드는 중입니다... 완료
상태 정보를 읽는 중입니다... 완료        
주의, './google-chrome-stable_current_amd64.deb' 대신에 'google-chrome-stable' 패키지를 선택합니다
다음 새 패키지를 설치할 것입니다:
  google-chrome-stable
0개 업그레이드, 1개 새로 설치, 0개 제거 및 0개 업그레이드 안 함.
0 바이트/95.0 M바이트 아카이브를 받아야 합니다.
이 작업 후 315 M바이트의 디스크 공간을 더 사용하게 됩니다.
받기:1 /root/다운로드/google-chrome-stable_current_amd64.deb google-chrome-stable amd64 113.0.5672.92-1 [95.0 MB]
Selecting previously unselected package google-chrome-stable.
(데이터베이스 읽는중 ...현재 205036개의 파일과 디렉터리가 설치되어 있습니다.)
Preparing to unpack .../google-chrome-stable_current_amd64.deb ...
Unpacking google-chrome-stable (113.0.5672.92-1) ...
google-chrome-stable (113.0.5672.92-1) 설정하는 중입니다 ...
update-alternatives: using /usr/bin/google-chrome-stable to provide /usr/bin/x-w
ww-browser (x-www-browser) in auto mode
update-alternatives: using /usr/bin/google-chrome-stable to provide /usr/bin/gno
me-www-browser (gnome-www-browser) in auto mode
update-alternatives: using /usr/bin/google-chrome-stable to provide /usr/bin/goo
gle-chrome (google-chrome) in auto mode
Processing triggers for gnome-menus (3.36.0-1ubuntu3) ...
Processing triggers for man-db (2.10.2-1) ...
Processing triggers for mailcap (3.70+nmu1ubuntu1) ...
Processing triggers for desktop-file-utils (0.26-1ubuntu3) ...
N: Download is performed unsandboxed as root as file '/root/다운로드/google-chrome-stable_current_amd64.deb' couldn't be accessed by user '_apt'. - pkgAcquire::Run (13: 허가 거부)
root@shinjaesang-virtual-machine:~/다운로드# nano google-chrome-stable
root@shinjaesang-virtual-machine:~/다운로드# nano /usr/bin/google-chrome-stable
root@shinjaesang-virtual-machine:~/다운로드# nano /usr/bin/google-chrome-stable
root@shinjaesang-virtual-machine:~/다운로드# google-chrome
[3585:3585:0516/104532.852786:ERROR:network_service_instance_impl.cc(541)] Network service crashed, restarting service.

(google-chrome:3585): IBUS-WARNING **: 10:46:02.857: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:02.863: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:02.990: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:03.804: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:03.816: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:03.881: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:03.980: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:03.985: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.044: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.116: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.118: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.172: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.484: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.488: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.549: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.588: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.594: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.708: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.740: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.742: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.812: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.852: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.853: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.972: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:04.975: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:05.014: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:05.075: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:05.788: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:05.816: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:09.447: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:09.451: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:19.638: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:20.741: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:20.745: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:20.844: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:20.851: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:20.924: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:21.036: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:21.037: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:21.040: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:21.164: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:21.565: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:21.620: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:21.708: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:21.766: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:21.844: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.108: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.540: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.543: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.620: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.626: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.684: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.789: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.790: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.868: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:22.956: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:23.020: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:23.116: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:23.180: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:23.653: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:23.788: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:23.932: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:23.980: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.036: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.140: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.145: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.173: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.174: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.177: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.215: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.284: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.320: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.325: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.421: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.426: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.431: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.524: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.580: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.584: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.670: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.702: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.708: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.804: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:24.853: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.353: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.384: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.414: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.444: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.473: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.503: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.534: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.565: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.595: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.625: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.656: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.686: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.717: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.748: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.774: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.775: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:25.892: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:26.020: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:26.044: google-chrome has no capability of surrounding-text feature

(google-chrome:3585): IBUS-WARNING **: 10:46:38.732: google-chrome has no capability of surrounding-text feature

^Croot@shinjaesang-virtual-machine:~/다운로드# ^C
root@shinjaesang-virtual-machine:~/다운로드# google-chrome
[4816:4831:0516/104731.219687:ERROR:command_buffer_proxy_impl.cc(128)] ContextResult::kTransientFailure: Failed to send GpuControl.CreateCommandBuffer.

^Croot@shinjaesang-virtual-machine:~/다운로드# bg
bash: bg: 현재: 그런 작업이 없음
root@shinjaesang-virtual-machine:~/다운로드# google-chrome
[5062:5078:0516/105024.593505:ERROR:command_buffer_proxy_impl.cc(128)] ContextResult::kTransientFailure: Failed to send GpuControl.CreateCommandBuffer.
^Z
[1]+  멈춤                  google-chrome
root@shinjaesang-virtual-machine:~/다운로드# bg
[1]+ google-chrome &
root@shinjaesang-virtual-machine:~/다운로드# [0516/105053.373586:ERROR:nacl_helper_linux.cc(355)] NaCl helper process running without a sandbox!
Most likely you need to configure your SUID sandbox correctly
