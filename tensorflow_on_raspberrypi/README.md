# tensorflow_on_raspberrypi

ラズパイ３上でtensorflowを使いたかったので、
tensorflowの環境を構築するためのDockerfileを作りました。

### 使い方

https://github.com/samjabrahams/tensorflow-on-raspberry-pi/releases

このリンク先から、必要なバージョンのwhlをダウンロードしておく必要があります。

現在、ここの`Dockerfile`では`tensorflow-1.1.0-cp34-cp34m-linux_armv7l.whl`を使うようになっていますが、

インストールしたいバージョンが違う場合は、`Dockerfile`を編集してファイル名を変更してください。

### 備考

下の参考リンクのように、raspberry pi上のtensorflowの環境構築をdockerでやっている例は見つかったのですが、
python3でやりたかったのと、最低限必要なモジュールだけインストールしたかったというのがあり、
Dockerfileを新たに作るに至りました。

と言っても、下のリンク先のDockerfileをほとんどパクっています。

### 参考

 * https://github.com/romilly/rpi-docker-tensorflow

 * https://github.com/samjabrahams/tensorflow-on-raspberry-pi
