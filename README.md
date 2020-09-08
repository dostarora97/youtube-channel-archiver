# Usage

*For Unix Like Systems*  

1. Put the url of channels that are to be archieved in `youtube-dl-channels.txt`  
2. Video Ids present in `youtube-dl-archive.txt` would not be downloaded.  
(This is to make sure videos are not downloaded multiple times if the script is rerun - since the id of every video that is downloaded will be written to `youtube-dl-archive.txt`)  
3. `chmod +x channel-archive.sh`
4. `./channel-archive.sh`

# Required
- ffmpeg/avconv (for post-download operations)
- AtomicParsley (To embed thumbnails)