# ubuntu-suffering
Repo created to reduce the suffering and pain on setting up ubuntu on PC


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
    sudo apt-get purge 'nvidia*'
    sudo add-apt-repository ppa:graphics-drivers
    sudo apt-get update
    sudo ubuntu-drivers autoinstall
 ~~~
 10) Reinicie o PC
 ~~~
    sudo reboot
 ~~~
 Agora tudo deve funcionar normalmente...

## LINKS UTEIS
 - https://forums.developer.nvidia.com/t/geforce-rtx-4060-not-working-with-ubuntu-20-04/249459/33
 - https://youtu.be/ADtRc_kA6Jw?si=sqlcWblJP4eVmpwm

