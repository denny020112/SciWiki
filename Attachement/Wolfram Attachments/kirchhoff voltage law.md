#Wolfram 
![[kirchhoff_voltage_law.png|400]]
```Wolfram
kvlCircuit = Graphics[{

  (* 배터리 *)

  Line[{{0, 0}, {0, 2}}],

  Line[{{-0.1, 0.4}, {0.1, 0.4}}],

  Line[{{-0.2, 0.6}, {0.2, 0.6}}],

  (* 저항 *)

  Line[{{0, 2}, {2, 2}}],

  Line[{{2, 2}, {2, 0}}],

  Line[{{2, 0}, {0, 0}}],

  (* 저항 표시 *)

  Rectangle[{0.8, 1.9}, {1.2, 2.1}],

  Rectangle[{1.9, 0.8}, {2.1, 1.2}],

  Rectangle[{0.8, -0.1}, {1.2, 0.1}],

  (* 전압 표시 *)

  Text[Style["V", 12], {-0.3, 1}],

  Text[Style["V1", 12], {1, 2.2}],

  Text[Style["V2", 12], {2.3, 1}],

  Text[Style["V3", 12], {1, -0.2}],

  (* 설명 *)

  Text[Style["Kirchhoff's Voltage Law (KVL)", Bold, 14], {1, -0.8}],

  Text[Style["Summation of total voltage in a closed circuit is 0:", 12], {1, -1.2}],

  Text[Style["V = V1 + V2 + V3", 12], {1, -1.6}]

},

  PlotRange -> {{-0.5, 2.5}, {-1.8, 2.5}},

  ImageSize -> 400

]

  

Export["kirchhoff_voltage_law.png", kvlCircuit]
```