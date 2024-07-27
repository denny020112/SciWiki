#Wolfram
![[kirchhoff_current_law_final.png]]
```Wolfram
kclCircuit = Graphics[{

  (* 노드 *)

  Disk[{0, 0}, 0.1],

  (* 전류 화살표 *)

  Arrow[{{0, 1}, {0, 0.1}}],  (* I1: 들어오는 전류 *)

  Arrow[{{-0.1, -0.05}, {-1, -0.5}}],  (* I2: 나가는 전류 *)

  Arrow[{{0.1, -0.05}, {1, -0.5}}],  (* I3: 나가는 전류 *)

  (* 전류 라벨 *)

  Text[Style["I1", 12], {0.2, 0.5}],

  Text[Style["I2", 12], {-0.7, -0.3}],

  Text[Style["I3", 12], {0.7, -0.3}],

  (* 설명 *)

  Text[Style["Kirchhoff's Current Law (KCL)", Bold, 14], {0, -1.2}],

  Text[Style["Current into the node = Current out of the node", 12], {0, -1.6}],

  Text[Style["I1 = I2 + I3", 12], {0, -2}]

},

  PlotRange -> {{-1.5, 1.5}, {-2.2, 1.2}},

  ImageSize -> 400

]

  

Export["kirchhoff_current_law_final.png", kclCircuit]
```