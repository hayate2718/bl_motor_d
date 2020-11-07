# ブラシレスモータドライバー基板
1. FETはTO252であれば使える。ゲート抵抗とゲートソース間コンデンサを調整すること。
2. vdsth_pinで短絡検出を行う。パルス電流の絶対最大定格時の電圧降下を入れればいいと思う。
3. ref_pinで定常の電流制限を行う。
https://latex.codecogs.com/gif.latex?\frac{5&space;\times&space;R1}{R1&plus;R2}&space;=&space;19&space;\times&space;R_{shunt}&space;\times&space;I_{max}
4. 一枚の値段がいくらになるのか考えたくもない...
5. untitl.txtファイルは読んでください
