# Unity Twitter 分享

[TOC]

## 插件功能

:::info
讓玩家能快速撰寫一篇Twitter推文，協助遊戲宣傳
:::

![](https://i.imgur.com/obfVxW3.png)


## 下載

- 在GitHub頁面下載`TwitterShare.unitypackage`
- 在Unity使用 Assets/import Package 打開。

## 專案架構

### 1.Sample(Scene)
- 範例場景，可以觀看插件如何運作
- 【按鈕】分享推文(無變數) : 使用 2.Twitter Share Manager(Script)
- 【按鈕】分享推文(有變數) : 使用  3.Twitter Share With Variable Manager(Script)


### 2.Twitter Share Manager(Script)

:::info
使用場合 : 當分享的推文中，不需要添增遊戲變數(分數、秒數)
:::

#### 貼文內容
![](https://i.imgur.com/jKJgcDJ.png)
- tweetMainContext : 主要推文撰寫區
    - 換行使用%0a
    - 請注意推文有140字限制
- GAME_LINK : 你的遊戲連結
- twittertags : 遊戲hashtags
    - 請使用,(逗號)隔開兩個hashtags


### 3.Twitter Share With Variable Manager(Script)
:::info
使用場合 : 當分享的推文中，需要添增遊戲變數(分數、秒數)
:::


#### 貼文內容
![](https://i.imgur.com/WdRaCUe.png)
- 推文中的遊戲變數 : 可自行在程式碼中添增變數
    - 範例: score=100，在推文中會顯示 (我打了100隻勞淑)
- tweetMainContext : 主要推文撰寫區
    - 請打開程式碼，在31行的tweetMainContext撰寫推文內容
    - ![](https://i.imgur.com/P0wz2dM.png)
- GAME_LINK : 你的遊戲連結
- twittertags : 遊戲hashtags
    - 請使用,(逗號)隔開兩個hashtags
