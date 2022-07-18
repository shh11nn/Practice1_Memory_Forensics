# 実習1 「Volatility Framework」によるメモリフォレンジック
Caineというフォレンジック専用のLinuxやWindows環境に直接ツールを導入して、フォレンジックの勉強をしていく。<br>
今回はVolatility Frameworkというツールを使いメモリフォレンジックを勉強をする。<br>
メモリフォレンジックとは電気が流れてないと覚えたことを忘れちゃうメモリ上のデータを解析する技術のことだ。<br>
[http://sectanlab.sakura.ne.jp/sendaictf/fyi.html](http://sectanlab.sakura.ne.jp/sendaictf/fyi.html)
![https://github.com/shh11nn/Practice1_Memory_Forensics/blob/main/sendai.png](https://github.com/shh11nn/Practice1_Memory_Forensics/blob/main/sendai.png)
# 事前準備
上記のリンクから講義資料や実習データはダウンロードして頂きたい。<br>
まずは自分の場合WindowsのPCなので、Windowsに実習データをダウンロードし、<br>
VirtualBoxの共有フォルダー機能を使い仮想環境上のCaineとリンクさせる。<br>
そして、実際に使えるようにするには指定されたパスでコマンドを打つ必要がある。<br>
![https://github.com/shh11nn/Practice1_Memory_Forensics/blob/main/sendai.png](https://github.com/shh11nn/Practice1_Memory_Forensics/blob/main/setting1.png)
![https://github.com/shh11nn/Practice1_Memory_Forensics/blob/main/sendai.png](https://github.com/shh11nn/Practice1_Memory_Forensics/blob/main/setting2.png)
# やること
①ネットワーク接続状況の確認<br>
②不審プロセスの確認<br>
攻撃者のC2サーバ「c2.hacker.com」から<br>
遠隔操作型マルウェアに感染し、内部の営業所の社員用PCとの間で不正通信が発生した。<br>
通信間にあるプロキシサーバのipは192.168.100.50でportは3128だ。<br>
感染した社員用PCのipは172.16.0.132だ。<br>

# ①ネットワーク接続状況の確認

# ②不審プロセスの確認
