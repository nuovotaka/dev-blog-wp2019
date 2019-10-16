+++
draft = false
slug = "mac-catalina-make-installmedia"
categories = ['mac']
tags = ['mac', 'installmedia']
date = "2019-10-10T10:30:00+09:00"
title = "備忘録 - MacOS Catalinaのインストールメディアの作成方法"

+++

もしものためにインストールUSBメディアを作成。
<!--more-->

### MacOS Catalinaをダウンロード

appストアよりダウンロードしてください。

### インストールUSBメディアの作成

使用するUSBメディアの容量を最低でも12GB以上の物を用意する。  
[【 サンディスク 正規品 】5年保証 USBメモリ 16GB USB 3.0 スライド式 SanDisk Ultra SDCZ48-016G-J57](https://amzn.to/31k0mVU)

#### ボリューム名の変更

「MyVolume」に変更しておきます。なんでもokです。

#### インストールメディアの作成

```
sudo /Applications/Install\ macOS\ Catalina.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume
```

ここで使っている```createinstallmedia```はmacOS Catalinaに付属のコマンドでappストアからOSをダウンロードして使えるコマンドになります。

### USBからの起動

Optionキーを押しながらMacを起動し「Install macOS Catalina」を選択。
