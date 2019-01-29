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
        url: 'http://211.97.73.147/amobile.music.tc.qq.com/C400002E3MtF0IAMMY.m4a?guid=4068577132&vkey=743DB8746F33CCC775C16AF43C46FE5F6DDFFADE0782EEAF9DB9021D4F87BCD7F181A6067ADDF7E3F468B510DCB508B5B6FC5ECA22AD04E0&uin=0&fromtag=66',
        cover: '//y.gtimg.cn/music/photo_new/T002R300x300M000001mTkmb4GJlh4.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '没有什么不同',
        artist: '曲婉婷',
        url: 'http://211.97.73.154/amobile.music.tc.qq.com/C400003gab3g2kUMwd.m4a?guid=3311042164&vkey=4CD46D32E139B4DA360E7B5FE03A4CA5946CADAE43D371B27F79F5B1B8017D6D7D431420CBBFB5B1C4270236C7A674A2923EBE0F67634A6C&uin=0&fromtag=66',
        cover: 'https://y.gtimg.cn/music/photo_new/T002R300x300M000001ZEgp33CTpK9.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        },
        {
        name: '一曲相思',
        artist: '半阳',
        url: 'http://211.97.73.155/amobile.music.tc.qq.com/C400002u0fTY2HoJJp.m4a?guid=2988268813&vkey=5979D49DE306C471E36B17725B2BBB2E5ABA20C85EEEB4D68DAB43C8CB944F9B66AFEEA59D98280535F1C63D813333B4AD59AF30DD4EA445&uin=0&fromtag=66',
        cover: 'https://y.gtimg.cn/music/photo_new/T001R300x300M0000013RsPD3Xs0FG.jpg?max_age=2592000',
        lrc: 'https://raw.githubusercontent.com/QingShaoXi/Blog_Album/master/music/gnzw.lrc',
        theme: '#ebd0c2',
        }
        
    ]
});
</script>
