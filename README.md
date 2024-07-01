# medical-videograbber
SDI video signal transcoder


sudo apt install ffmpeg

v4l2-ctl --list-devices

ffmpeg -f v4l2 -i /dev/video2 -t 10 ordinace.mkv

rm /home/fedurca/out_test.mp4; 

ffmpeg -i /home/fedurca/ordinace2.mkv -vf "drawtext=text='860804/8556':fontfile=/usr/share/fonts/truetype/ubuntu/UbuntuMono-R.ttf:fontsize=26:fontcolor=white:x=170:y=17,drawtext=text='Luděk Fedurca':fontfile=/usr/share/fonts/truetype/ubuntu/UbuntuMono-R.ttf:fontsize=26:fontcolor=yellow:x=170:y=47,drawtext=text='Luděk Fedurca':fontfile=/usr/share/fonts/truetype/ubuntu/UbuntuMono-R.ttf:fontsize=26:fontcolor=red:x=170:y=138,drawtext=text='M':fontfile=/usr/share/fonts/truetype/ubuntu/UbuntuMono-R.ttf:fontsize=26:fontcolor=blue:x=105:y=138,drawtext=text='Luděk Fedurca':fontfile=/usr/share/fonts/truetype/ubuntu/UbuntuMono-R.ttf:fontsize=26:fontcolor=green:x=170:y=438"  /home/fedurca/out_test.mp4; 
vlc /home/fedurca/out_test.mp4
