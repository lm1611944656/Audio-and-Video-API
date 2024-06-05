# Audio-and-Video-API
由于网易云音乐API窗口被封，导致不能开发音乐播放器。至此查找到一个好用的API接口供大家使用。

参考地址:[github][1]

# 一、酷狗使用教程

```html
https://dataiqs.com/api/kgmusic/?msg=出现又离开&type&n=5
```

>https://dataiqs.com/api/kgmusic/   
>
>**后面的 ? 表示查询字符串，字符串与字符串之间用 & 分隔开。**
>
>查询字符串的常见用途包括：
>
>1. 向服务器传递用户输入的数据。
>2. 根据不同的参数获取不同的数据。
>3. 进行分页、过滤和排序操作。

- msg是key，"出现又离开"是value
  - 出现又离开还是客户想要查询的歌曲

- type是key
  - value可以为null
  - value可以为**mv**
  - value可以为**song**

- id是key
  - value可以为null
  - value可以为歌曲id

- n是key
  - value可以是null
  - value可以是0~9的数(表示获取酷狗音乐播放界面上第几位歌手的音频和视频)；0表示第0位歌手唱的音频和视频分别对应的url。

## 1.1 实例案例

随机输出热歌榜歌单歌曲

```
https://dataiqs.com/api/netease/music/?type=random&id=
```

## 1.2 实际案例

搜索“后来”，type不限制(可以是音频，也可以是视频)，歌手是第5位。

```http
https://dataiqs.com/api/netease/music/?msg=后来&type&n=5
```



# 二、网易使用教程

网易API使用教程和酷狗类似，在此不做赘述。

[1]: https://github.com/ihmily/music-api





