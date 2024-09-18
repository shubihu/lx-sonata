# lx-sonata
 基于开源音乐软件lx-music进行二次封装的sonata定制版。
 - 感谢lx-music的开源（https://github.com/lyswhut/lx-music-mobile）
 - 使用本软件同样需遵循洛雪的相关相关协议。
 - 洛雪源码使用方法：https://lxmusic.toside.cn/mobile/use-source-code

## 主要修改的内容
依赖包React Native Track Player的源码(MusicManager.java)
```
// player.setAudioAttributes(new androidx.media3.common.AudioAttributes.Builder()
//         .setContentType(C.AUDIO_CONTENT_TYPE_MUSIC).setUsage(C.USAGE_MEDIA).build(), shouldHandleAudioFocus);

player.setAudioAttributes(new androidx.media3.common.AudioAttributes.Builder()
           .setContentType(C.CONTENT_TYPE_MUSIC).setUsage(C.USAGE_ASSISTANCE_NAVIGATION_GUIDANCE).build(),false);
```
