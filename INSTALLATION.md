# Installation 

So far Dejavu has only been tested on Unix systems.

* [`pyaudio`](http://people.csail.mit.edu/hubert/pyaudio/) for grabbing audio from microphone
* [`ffmpeg`](https://github.com/FFmpeg/FFmpeg) for converting audio files to .wav format
* [`pydub`](http://pydub.com/), a Python `ffmpeg` wrapper
* [`numpy`](http://www.numpy.org/) for taking the FFT of audio signals
* [`scipy`](http://www.scipy.org/), used in peak finding algorithms
* [`matplotlib`](http://matplotlib.org/), used for spectrograms and plotting
* [`MySQLdb`](http://mysql-python.sourceforge.net/MySQLdb.html) for interfacing with MySQL databases



## Centos/Fedora 20+

### Dependency installation on Fedora 20+

1.Install the dependencies:

    sudo yum install numpy scipy python-matplotlib ffmpeg portaudio-devel
    pip install PyAudio
    pip install pydub
    pip install ffmpy
    pip install psycopg2
    
2.For database: 
    
    1.Pgsql only supported:
    2.create a database manually for example: shazam
    3.At the begining comment the code  in dejavu/__init__.py line no 46.
    4.Execute " python dejavu/truncate.py " on shell , will create the tables for you
    5.Uncomment the code  in dejavu/__init__.py line no 46.

    
    


