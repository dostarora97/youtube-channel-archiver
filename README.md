# Usage

*For Unix Like Systems*  

1. Put the urls of channels that are to be downloaded in `youtube-dl-channels.txt` line-wise   
3. `chmod +x channel-archive.sh`
4. `./channel-archive.sh`

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/dostarora97/youtube-channel-archiver/blob/master/colab/Youtube_Channel_Archiver.ipynb)


# Required
- youtube-dl
- ffmpeg (for post-download operations)
- ~~AtomicParsley (To embed thumbnails)~~
```
sudo apt update -y
sudo apt install ffmpeg
sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
sudo chmod a+rx /usr/local/bin/youtube-dl
```
  
# Note
- Video Ids present in `youtube-dl-archive.txt` would **NOT** be downloaded.
- By default, this file is kept empty on the first run.
- As the download progresses the videos Ids are written to `youtube-dl-archive.txt`

This is to make sure videos are not downloaded multiple times if the script is rerun.