# ブラシレスモータドライバー基板<br>
1.  FETはTO252であれば使える。ゲート抵抗とゲートソース間コンデンサを調整すること<br>
vdsth_pinで短絡検出を行う。パルス電流の絶対最大定格時の電圧降下を入れればいいと思う。<br>
ref_pinで定常の電流制限を行う。計算式は下記の通り <br>
<div align = "center">
<img src = "https://latex.codecogs.com/gif.latex?\frac{5&space;\times&space;R1}{R1&plus;R2}&space;=&space;19&space;\times&space;R_{shunt}&space;\times&space;I_{max}">
</div>
一枚の値段がいくらになるのか考えたくもない...<br>
untitl.txtファイルは読んでください
