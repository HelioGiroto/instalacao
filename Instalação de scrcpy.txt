https://www.tomshardware.com/how-to/control-android-device-from-pc-using-scrcpy
https://duckduckgo.com/?q=scrcpy&ia=web
https://github.com/Genymobile/scrcpy?tab=readme-ov-file
https://github.com/Genymobile/scrcpy/blob/master/doc/linux.md
https://duckduckgo.com/?q=tradutor+google&ia=web



# Sobre desbloquear o telefone para habilitá-lo:

	Configurações > Sobre o Telefone > Informações do software > Número de compilação 
	Toque 7 vezes
	MSG: "O modo de desenvolvedor foi ativado"
	
	Volta à Configurações > Opções do desenvolvedor > Em Depuração: Depuração USB ativada (azul) > Conecta celular no USB e Permite



# INSTALAÇÃO:

Fonte - https://github.com/Genymobile/scrcpy/blob/master/doc/linux.md

Latest version
However, the packaged version is not always the latest release. To install the latest release from master, follow this simplified process.

First, you need to install the required packages:


# for Debian/Ubuntu
sudo apt install ffmpeg libsdl2-2.0-0 adb wget gcc git pkg-config meson ninja-build libsdl2-dev libavcodec-dev libavdevice-dev libavformat-dev libavutil-dev libswresample-dev libusb-1.0-0 libusb-1.0-0-dev
                 

Then clone the repo and execute the installation script (source):

git clone https://github.com/Genymobile/scrcpy
cd scrcpy
./install_release.sh

When a new release is out, update the repo and reinstall:

git pull
./install_release.sh



Run
Make sure that your device meets the prerequisites.

Once installed, run from a terminal:

scrcpy
or with arguments (here to disable audio and record to file.mkv):

scrcpy --no-audio --record=file.mkv
Documentation for command line arguments is available:

man scrcpy
scrcpy --help
on github




