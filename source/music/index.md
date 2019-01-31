---
title: 享受一下音乐，继续前行
date: 2019-01-24 15:21:19
type: music
---
<style>
#aplayer{ margin:0 auto; width:320px; height:100px; border:1px solid #F00}
</style>
<br>
<br>
<!--音乐-->
<link rel="stylesheet" href="https://cdn.bootcss.com/aplayer/1.10.1/APlayer.min.css">
<div id="aplayer" style="z-index:9999;"></div>
<script src="../assets/js/APlayer.min.js"></script>
<script>
const ap = new APlayer({
    container: document.getElementById('aplayer'),
    fixed: true,
    autoplay: true,
    theme: '#b7daff',
    loop: 'all',
    preload: 'auto',
    mutex: true,
    volume: 0.7,
    lrcType: 3,
    listFolded: true,
    listMaxHeight: '150px',
    audio: [
        {
        name: '光年之外',
        artist: '邓紫棋',
        url: 'http://fs.w.kugou.com/201901300856/ec302bec1b40685c281f84259d4dc739/G083/M08/00/04/84YBAFhks0aAYGsBADl8RUL2DXQ825.mp3',
        cover: '//y.gtimg.cn/music/photo_new/T002R300x300M000001mTkmb4GJlh4.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '没有什么不同',
        artist: '曲婉婷',
        url: 'http://fs.w.kugou.com/201901300947/1fd0a06c6c93000a8099dba13bc18089/G009/M08/18/18/SQ0DAFUOaXOAeDyiAEZlOWt47Lw378.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T002R300x300M000001ZEgp33CTpK9.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '一曲相思',
        artist: '半阳',
        url: 'http://fs.w.kugou.com/201901300842/837c15f2c52656b0aeb689c3c4487cea/G085/M07/0B/10/lQ0DAFujV42AK4xpACkHR2d9qTo587.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '一路之下',
        artist: '张杰',
        url: 'http://fs.w.kugou.com/201901301048/2300f784faf7d4e45235ab6c26de86ae/G121/M03/13/03/GYcBAFxQWO-AHwGWADinswYlBJ8886.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '告白气球',
        artist: '周杰伦',
        url: 'http://fs.w.kugou.com/201901301100/338bd170879113050849c04deb409057/G063/M03/06/11/34YBAFdskzmAUMlOADSMOxgm3l4714.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '安静',
        artist: '周杰伦',
        url: 'http://fs.w.kugou.com/201901301040/5e39cbe5e4e51ee51a7e8c35ebacf239/G005/M07/1A/08/pYYBAFT-yCGAR2AuAFHzeoODc5k446.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '月半小夜曲',
        artist: '李克勤',
        url: 'http://fs.w.kugou.com/201901301054/e7d4b205e3d6886f157c41b4848e569a/G012/M05/1A/09/TA0DAFUOAaiAD4dMAEccEw4b070166.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '相依为命',
        artist: '陈小春',
        url: 'http://fs.w.kugou.com/201901301025/29a6c582929af6a65e4fc0f935b0b813/G012/M06/0D/17/rIYBAFUN3hOAA_V7ADoTth0Vuio226.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '蓝莲花',
        artist: '许巍',
        url: 'http://fs.w.kugou.com/201901301057/47d6048fe8c426b633ad9dce2a35b9a4/G008/M08/07/04/SA0DAFT7mn6AVDw6AEIXhTXgYbw529.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '偷走',
        artist: '萧煌奇',
        url: 'http://fs.w.kugou.com/201901301125/127a3dcd64b697fbd11b0b7254fdf692/G057/M02/0E/04/eQ0DAFcGjBOAAjAyADt2JxWuZ7g806.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '末班车',
        artist: '萧煌奇',
        url: 'http://fs.w.kugou.com/201901301126/5fc2a0bf300b9f8100a7a48f99cd72f4/G005/M05/00/01/RQ0DAFS28F2AaI3UAEaFwOkauSA733.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '停了的钟',
        artist: '萧煌奇',
        url: 'http://fs.w.kugou.com/201901301127/cd234c69b479f6813b823d6f3bd9bc38/G059/M00/08/11/ew0DAFcGjBGAL2Q9AEUhRWzdkYs445.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '倒数',
        artist: '邓紫棋',
        url: 'http://fs.w.kugou.com/201901301116/f631e6026433d76e3ff28c2d7a8a9de1/G138/M01/19/08/apQEAFtrn3aACm3MADgCIaT4E1Q056.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '雨蝶',
        artist: '邓紫棋&张靓颖',
        url: 'http://fs.w.kugou.com/201901301130/c7955e716a542f9e949281e95a721c74/G127/M03/06/17/H4cBAFqrnPOALv7xAD46ab3Mw00584.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '终于等到你',
        artist: '张靓颖',
        url: 'http://fs.w.kugou.com/201901301125/8d4af09b5dabd2c53e8b6cd0c3311e43/G013/M03/1A/01/rYYBAFUJf9-AF4DWAEgYPdZoZ-E939.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '我的梦',
        artist: '张靓颖',
        url: 'http://fs.w.kugou.com/201901301121/b7a565649f3be3dbf0be589cf7255adb/G147/M07/1A/15/c5QEAFvedoWANDQTADWd4uKEOFk655.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '如果这就是爱情',
        artist: '张靓颖',
        url: 'http://fs.w.kugou.com/201901301011/9445210ed57f93d639e49d38345d5863/G003/M09/0E/13/Qw0DAFT8QdeAbsdQAEUMvE95Neo115.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '无地自容',
        artist: '黑豹乐队',
        url: 'http://fs.w.kugou.com/201901301005/00256645ce7538bfbd9b865893d308a3/G010/M06/11/01/Sg0DAFUGqEeAPUr4AFMfGUJ2DLc793.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '山高路远',
        artist: '谭维维',
        url: 'http://fs.w.kugou.com/201901301134/2792224c2a59bd2f3606121d8f417834/G128/M07/01/13/wA0DAFxMMOaACb-wAEKnM6HAalU479.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '真的爱你',
        artist: 'beyond',
        url: 'http://fs.w.kugou.com/201901301105/cff0050b414b277766554d6416517859/G135/M03/10/0F/J4cBAFuGdRiAT-jCAEOVZVhv24s616.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '千千厥歌',
        artist: '程慧贤',
        url: 'http://fs.w.kugou.com/201901301103/9acf12542cb2a310782c8c1f8917395b/G005/M07/19/10/pYYBAFS27HWAWEDXAEkuMomI9uE304.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '风的季节',
        artist: 'soler',
        url: 'http://fs.w.kugou.com/201901301131/129550f2d6895fd7422411e612d713c2/G012/M02/15/18/TA0DAFUAoxiAbyx1ADz2IQclDwU211.mp3',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        }
        
    ]
});
</script>
