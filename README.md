# Continuous-image-trajectory-record-support

連続画像データにおける特定のオブジェクトのX,Y座標をクリック連打で記録して軌跡をCSVに保存する支援ソフト

##使い方

前提：コンパイルして実行する場合はHSPが必要です。>http://hsp.tv/

exeの動作環境は、多分Windows95～Windows10, Wineもいけるはずです。//開発Windows10

1. 動画ファイルをffmpegなどを用いて連番データにしてフォルダにまとめる
`ffmpeg -i hoge.mp4 images/%06d.jpg`
2. このソフトを開き、フォルダ画像を1つ選ぶ（フォルダ指定のため）
3. 追跡したいものをひたすらクリックしていく。クリックしっぱなしで2fpsくらいでクリックを適用していくバーストモードがある。
4. 間違えた場合は右クリックをすると1フレーム戻る
5. 最終成果物はCSVに保存させる(強制)

##注意

途中で保存するなどといった気の利いたシステムは無いので、事故に注意。HSPで書いてあるからまあ、書けるでしょ？　12歳以上なんだし（煽り）
