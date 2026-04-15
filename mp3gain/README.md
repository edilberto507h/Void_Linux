MP3Gain
Analyzes and adjusts the volume of MP3 files

MP3Gain analyzes and losslessly adjusts mp3 files to a specified target volume.
It does not simply do peak amplitude normalization. Instead, it performs statistical analysis to determine how loud the file actually sounds to the human ear.

How to compile mp3gain for Void Linux

sudo xbps-install -S base-devel mpg123 mpg123-devel unzip wget

wget -c https://github.com/edilberto507h/Void_Linux/raw/refs/heads/main/mp3gain/mp3gain-src.zip

unzip mp3gain-src.zip

cd mp3gain-src

make 

sudo cp mp3gain /usr/local/bin/


How to compile wxmp3gain for Void Linux

sudo xbps-install -S base-devel cmake gtk+3-devel wxWidgets-devel unzip wget

wget -c https://github.com/edilberto507h/Void_Linux/raw/refs/heads/main/mp3gain/wxmp3gain.zip

unzip wxmp3gain.zip

cd wxmp3gain

mkdir build

cd build

cmake .. -DwxWidgets_CONFIG_EXECUTABLE=/usr/bin/wx-config-gtk3

make -j$(nproc)

sudo make isntall




