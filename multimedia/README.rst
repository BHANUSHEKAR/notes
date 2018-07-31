========================================
多媒體 (Multimedia)
========================================


.. contents:: 目錄


基本概念、格式
========================================

* `基本觀念 <concept.rst>`_
    - Video
    - Audio
    - Codec
    - Container
    - Operations
        + Transcoding
        + Transmuxing
        + Transrating
        + Transsizing
        + Adaptive Streaming
* `Audio <audio.rst>`_
    - No Compression
        + PCM
        + LPCM
    - Lossless Compression
        + FLAC
        + ALAC
        + MLP/Dolby TrueHD
        + DTS-HD
    - Lossy Compression
        + MP3
        + WMA
        + Vorbis
        + Opus
        + AAC
        + AC-3
        + DTS
* `Video <video.rst>`_
    - MPEG-1
    - MPEG-2
    - MPEG-4 (A)SP
    - H.264/MPEG-4 AVC
    - H.265/HEVC
    - VC-1/WMV
    - Real Video
    - Theora
    - Microsoft MPEG4 V2
    - VP8
    - VP9
    - MVC
    - AV1
* `Media Container <media-container.rst>`_
    - AVI
    - FLV
    - QuickTime
    - MP4
    - MPEG-TS
    - Ogg
    - Matroska
* `降噪 (Noise Cancellation) <noise-cancellation.rst>`_
    - Active Noise Cancellation
    - Passive Noise Cancellation
    - SNR (Signal to Noise Ratio)
    - Common Noise Types
        + Echo
        + Siren
        + Crowd
        + Beep
        + Airport
        + Coffeeshop
        + Street
* `Video Quality <video-quality.rst>`_
* `SDP (Session Description Protocol) <sdp.rst>`_
* `PTS/DTS (Presentation Timestamp/Decode Timestamp) <pts-dts.rst>`_
* I-frame/P-frame/B-frame
* Synchronization



架構、工具
========================================

* `Linux Sound System <linux-sound-system.rst>`_
* ALSA
* `PulseAudio <pulseaudio.rst>`_
* JACK
* `GStreamer <gstreamer.rst>`_
    - 基本介紹、設計概念
    - 內部溝通機制
    - 撰寫 Plugin
    - Transcoding
    - Transmuxing
    - Transrating
    - Transsizing
    - Adaptive Streaming
    - File Repair
    - WebRTC
    - UPnP streaming
    - DLNA
    - Miracast
    - Google Cast
    - Bluetooth
    - Player
    - Server
    - Filter
    - 上字幕
    - `GStreamer 相關公司 <gstreamer/company.rst>`_
* `FFmpeg <ffmpeg.rst>`_
    - CLI 參數使用
    - Transcoding
    - Transmuxing
    - Transrating
    - Transsizing
    - Adaptive Streaming
    - File Repair
    - Filter
    - 上字幕
    - 架構設計
        + Encoder
        + Decoder
        + Muxer/Demuxer
    - 元件用途
        + libavutil
        + libavcodec
        + libavformat
        + libavdevice
        + libavfilter
        + libavresample
        + libswscale
        + libswresample
        + libpostproc
    - C API
    - 其他程式語言 Binding
    - 硬體加速
    - Player
    - Server
* `OpenCV <opencv.rst>`_
* `WebRTC <webrtc.rst>`_
* `MediaInfo <mediainfo.rst>`_
* `硬體加速 <hardware-acceleration.rst>`_
* AudioFlinger



給 End User 的軟體
========================================

* `播放器 <player.rst>`_
    - VLC
    - mplayer
    - mpv
    - cmus
    - GStreamer (gst-play-1.0)
    - FFmpeg (ffplay)
    - mpd
    - Mopidy
* `Kodi <kodi.rst>`_



其他
========================================

* 猜測多媒體格式
    - GStreamer typefind
