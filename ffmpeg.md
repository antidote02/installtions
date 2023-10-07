## FFmpeg入门
**官网：https://ffmpeg.org/**  
**维基：https://trac.ffmpeg.org/**
#### Scoop安装/升级FFmpeg
`scoop install -k ffmpeg`  
`scoop update -k ffmpeg`
#### FFmpeg
* `mp4.bat`
  ```
  ffmpeg -i %1 -c copy %~n1.mp4
  ```
* `aac.bat`
  ```
  ffmpeg -i %1 -c copy -vn %~n1.aac
  ```

**To be continued...**