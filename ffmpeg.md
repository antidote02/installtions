## FFmpeg入门
**官网：https://ffmpeg.org/**  
**维基：https://trac.ffmpeg.org/**
#### Scoop安装/升级FFmpeg
`scoop install -k ffmpeg`  
`scoop update -k ffmpeg`
#### FFmpeg
* `ffmpeg -i %1 -c copy %~n1.mp4`
* `ffmpeg -i %1 -c:v libx264 -x264opts opencl -crf 22 -preset veryslow -profile:v high -c:a copy -movflags faststart -threads 32 %~n1.mp4`
  * `ffmpeg -i %1 -vf scale=1920:1080 -c:v libx264 -x264opts opencl -crf 22 -preset veryslow -profile:v high -c:a copy -movflags faststart -threads 32 -fs 8G %~n1.mp4`

**To be continued...**