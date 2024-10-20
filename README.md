# ubuntu-suffering
Repo created to reduce the suffering and pain on setting up ubuntu on PC
UBUNTU SHOULD BE 22 LTS because there is no nvidia drivers for RTX 4050 on Ubuntu 24 LTS

 1) Abrir espaço no disco do WINDOWS<br>
 1.1) Tenha certeza de que o espaço separado esteja LIMPO e LIVRE
 2) Baixar o Linux LTS
 3) Criar um PENDRIVE BOOTAVEL
 4) BOOTAR o PENDRIVE pela BIOS e selecionar o pendrive
 5) Instalar o UBUNTU ALONGSIDE WINDOWS
 6) Ao abrir o UBUNTU, antes do login, vá em configurações e selecione UBUNTU ON WAYLANDS
 7) Agora entre no safe-mode "crlt + alt + f2"
 8) Faça o login normalmente
 9) Desinstale os drivers conflituosos da NVIDIA, adicione o repositorio da NVIDIA, atualize o repositorio e reinstale os driver da placa de video
 ~~~
   sudo apt-get remove --purge '^nvidia-.*'
   sudo apt-get remove --purge nvidia*
   sudo apt-get remove --purge xserver-xorg-video-nouveau
   sudo apt-get autoremove
   sudo apt-get autoclean
 ~~~
 10) Reinicie o PC
 ~~~
   sudo add-apt-repository ppa:graphics-drivers/ppa
   sudo apt update
   sudo reboot
 ~~~
 11) No Software & Updates >> Aditional Drivers voce verá que estará no X.orgs Nouveau. Migre para a versão 560 OPEN.

 Incertezas: Nos testes, eu coloquei a Nouvea em blacklist pois surgium um B.O do naipe "Conflict nouveau bond blabla"
 https://chatgpt.com/share/6715894f-b478-8007-a313-32a7fcad56c6
 

## LINKS UTEIS
 - https://forums.developer.nvidia.com/t/geforce-rtx-4060-not-working-with-ubuntu-20-04/249459/33
 - https://youtu.be/ADtRc_kA6Jw?si=sqlcWblJP4eVmpwm

