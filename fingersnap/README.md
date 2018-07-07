# fingersnap

↓ これを実現させるためにraspberry piに必要な環境構築したときのDockerfileです。

https://github.com/sana37/sound_recognition#%E4%BD%BF%E7%94%A8%E4%BE%8B

このDockerfileは、`tensorflow_on_raspberrypi`のDocker imageを継承してbuildを行います。

### モジュール

 * `python3-scipy`

  * 音声データをフーリエ変換するのに使う

 * `pyaudio`

  * USBマイクから音声データを取得するのに使う

 * `python3-serial`

  * ラズパイからマイコンにシリアル通信で信号を送るのに使う
