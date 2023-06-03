# AI_StackChan2_ut_custom

AIｽﾀｯｸﾁｬﾝ2を少しカスタムするために作ったforkです。
極力元のコードはそのままに、欲しい機能を追加してます。

## カスタム実装済み

- オリジナルの顔を追加
  - m5stack-avatar-ut-customのaa-face (`・ω・´)
- Bボタンで顔変更の追加
- 顔変更設定用のHTMLの追加
  - http://xxx.xxx.xxx.xxx/setting?face={番号}
  - 番号は0以上の数字、存在しない番号は Out of Indexと表示される。
    - 0 : 標準の顔 [・＿・]
    - 1 : AA顔 (`・ω・´)
- Wifi設定用のHTMLの追加
  - http://xxx.xxx.xxx.xxx/wifi

- その他の微調整
  - platformio.ini
    - ビルド対象を個別に指定する形（default_envsで指定）に変更


---

以下オリジナルのReadme

<br><br>

![画像1](images/image1.png)<br><br>

AIｽﾀｯｸﾁｬﾝ2の特徴<br>

* 音声合成にWeb版 VOICEVOXを使います。
* 音声認識に"Google Cloud STT"か"OpenAI Whisper"のどちらかを選択できます。
<br>

Google Cloud STTは、”MhageGH”さんの [esp32_CloudSpeech](https://github.com/MhageGH/esp32_CloudSpeech/ "Title") を参考にさせて頂きました。ありがとうございました。<br>
"OpenAI Whisper"が使えるようにするにあたって、多大なご助言を頂いた”イナバ”さん、”kobatan”さんに感謝致します。<br>

---


### M5GoBottom版ｽﾀｯｸﾁｬﾝ本体を作るのに必要な物、及び作り方 ###
こちらを参照してください。<br>
* [ｽﾀｯｸﾁｬﾝ M5GoBottom版組み立てキット](https://raspberrypi.mongonta.com/about-products-stackchan-m5gobottom-version/ "Title")<br>

### プログラムをビルドするのに必要な物 ###
* [M5Stack Core2](http://www.m5stack.com/ "Title")<br>
* VSCode<br>
* PlatformIO<br>

使用しているライブラリ等は"platformio.ini"を参照してください。<br>

~~【5/31の時点ではM5Unifiedの不具合の為、CoreS3では動きません。】~~<br>

---

### サーボモーターを使用するGPIO番号の設定 ###
* main.cppの46行目付近、サーボモーターを使用するGPIO番号を設定してください。


### 使い方 ###

こちらを参照してください。<br>

* [AI_StackChan2_README](https://github.com/robo8080/AI_StackChan2_README/ "Title")<br>
<br>
<br>
<br>
