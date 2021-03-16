# ブラシレスモータドライバー基板
## 機能
1. FETはTO252であれば使える。ゲート抵抗とゲートソース間コンデンサを調整すること<br>
ゲートソース間コンデンサは<img src = "https://latex.codecogs.com/gif.latex?\frac{C_{dg}}{C_{gs}}=0.5"> くらいになるようにする。
2. vdsth_pinで短絡検出を行う。パルス電流の絶対最大定格時の電圧降下を入れればいいと思う。計算式は下記 
<p align = "center"><img src = "https://latex.codecogs.com/gif.latex?V_{cc}\times\frac{R_1}{R_1&plus;R_2}=V_{ds(max)}"></p>

3. ref_pinで定常の電流制限を行う。計算式は下記 
<p align = "center"><img src = "https://latex.codecogs.com/gif.latex?\frac{5&space;\times&space;R1}{R1&plus;R2}&space;=&space;19&space;\times&space;R_{shunt}&space;\times&space;I_{max}"></p>

4. ピンヘッダをショートすることで動作モードの切り替えが可能<br>
jp1がfフラグを無視（オープンループでリミットを完全に外す場合はさらにRCピンをショートしてください）、jp2が高速減衰モードにできる(動くときと動かんときがある)
5. untitl.txtファイルは読んでください<br>
## 制作者コメント
<b>一枚の値段がいくらになるのか考えたくもない...結果としては4000yenほど(たけぇ<br>
このMDは制御方法が台形120度通電であるため低速域よりも高速域の効率のほうが良い。<br>
モータの最大効率運転では電流波形が正弦波に近いほどよく、台形120度通電では電流波形が台形になるように制御されているが高速域では電流波形が正弦波に近くなるため効率が良くなる。</b>
