# ブラシレスモータドライバー基板<br>
1. FETはTO252であれば使える。ゲート抵抗とゲートソース間コンデンサを調整すること<br>
ゲートソース間コンデンサは<img src = "https://latex.codecogs.com/gif.latex?\frac{C_{dg}}{C_{gs}}=0.5">くらいになるようにする。<br>
2. vdsth_pinで短絡検出を行う。パルス電流の絶対最大定格時の電圧降下を入れればいいと思う。計算式は下記の通り<br>
<div align = "center">
<img src = "https://latex.codecogs.com/gif.latex?V_{cc}\times\frac{R_1}{R_1&plus;R_2}=V_{ds(max)}">
</div>
3. ref_pinで定常の電流制限を行う。計算式は下記の通り <br>
<div align = "center">
<img src = "https://latex.codecogs.com/gif.latex?\frac{5&space;\times&space;R1}{R1&plus;R2}&space;=&space;19&space;\times&space;R_{shunt}&space;\times&space;I_{max}">
</div><br>
4. ピンヘッダをショートすることで動作モードの切り替えが可能
jp1がfフラグを無視（オープンループでリミットを完全に外す場合）、jp2が高速減衰モードにできる(動くときと動かんときがある)<br>
5. untitl.txtファイルは読んでください<br>
<b>一枚の値段がいくらになるのか考えたくもない...</b>
