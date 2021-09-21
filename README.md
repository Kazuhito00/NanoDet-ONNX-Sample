# NanoDet-ONNX-Sample
[NanoDet](https://github.com/RangiLyu/nanodet)のPythonでのONNX推論サンプルです。<br>
ONNXに変換したモデルも同梱しています。変換自体を試したい方は[Convert2ONNX.ipynb](Convert2ONNX.ipynb)を使用ください。<br>

https://user-images.githubusercontent.com/37477845/133836811-3f5ec972-a0e9-46e0-99e4-ad4e6adccade.mp4

# Requirement 
* OpenCV 3.4.2 or later
* onnxruntime 1.5.2 or later
* Pytorch 1.7 or later ※ONNX変換を実施する場合のみ
* pytorch-lightning 1.4.7 or later ※ONNX変換を実施する場合のみ

# Demo
デモの実行方法は以下です。
```bash
python sample_onnx.py
```
* --device<br>
カメラデバイス番号の指定<br>
デフォルト：0
* --movie<br>
動画ファイルの指定 ※指定時はカメラデバイスより優先<br>
デフォルト：指定なし
* --image<br>
画像ファイルの指定 ※指定時はカメラデバイスや動画より優先<br>
デフォルト：指定なし
* --width<br>
カメラキャプチャ時の横幅<br>
デフォルト：960
* --height<br>
カメラキャプチャ時の縦幅<br>
デフォルト：540
* --model<br>
ロードするモデルの格納パス<br>
デフォルト：model/nanodet_m_320.onnx
* --input_shape<br>
モデルの入力サイズ<br>
デフォルト：320
* --score_th<br>
クラス判別の閾値<br>
デフォルト：0.35
* --nms_th<br>
NMSの閾値<br>
デフォルト：0.6

# Reference
* [RangiLyu/nanodet](https://github.com/RangiLyu/nanodet)

# Author
高橋かずひと(https://twitter.com/KzhtTkhs)
 
# License 
NanoDet-ONNX-Sample is under [Apache-2.0 License](LICENSE).

# License(Movie)
サンプル動画は[NHKクリエイティブ・ライブラリー](https://www.nhk.or.jp/archives/creative/)の[イギリス ウースターのエルガー像](https://www2.nhk.or.jp/archives/creative/material/view.cgi?m=D0002011239_00000)を使用しています。
