# movie
视频相关资料收集
#videojs
videojs资料收集整理
# cdn #
<link href=”http://vjs.zencdn.net/c/video-js.css” rel=”stylesheet”>
<script src=”http://vjs.zencdn.net/c/video.js”></script>
# cdn ## end #
#标准页面创建#
<video id=”my_video_1″ class=”video-js vjs-default-skin” controls preload=”auto” width=”640″ height=”264″ poster=”my_video_poster.png” data-setup=”{}”>
<source src=”my_video.mp4″ type=’video/mp4′>
<source src=”my_video.webm” type=’video/webm’>
</video>

#接口api#
###获取对象 
var myPlyer = _V_("my_video_1");
###播放
myPlyer.play();
###暂停
myPlyer.pause();
###获取播放进度
var whereYouAre = myPlyer.currentTime();
###设置播放进度
myPlyer.currentTime(120);
###视频持续时间，加载完成视频才知道视频时长，且在flash情况下无效
var howLongIs = myPlayer.duration();
###缓冲，指下载了多少
var whatHasBeenBuffered = myPlyer.buffered();
var howMuchIsDownloaded = myPlayer.bufferedPercent(); //百分比的缓冲
###声音大小（0-1之间）
var howMuchIsDownloaded = myPlayer.volume();
###设置声音大小
myPlayer.volume(0.5);
###设置大小
myPlayer.size(640,480);
###全屏
myPlayer.enterFullScreen();
