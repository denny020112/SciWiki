#Wolfram 
![[electric_potential_2d.gif]]
```Wolfram
(* 상수 정의 *)

k = 9*10^9; (* 쿨롱 상수 *)

q1 = 1*10^-12; (* 고정된 점전하의 전하량 *)

q2 = 1*10^-12; (* 이동하는 점전하의 전하량 *)

  

(* 전기 퍼텐셜 에너지 함수 *)

potentialEnergy[r_] := k * q1 * q2 / r

  

(* 애니메이션 프레임 생성 *)

frames = Table[

  Show[

    (* 전기장 표현 *)

    VectorPlot[{x/(x^2 + y^2)^(3/2), y/(x^2 + y^2)^(3/2)}, {x, -10, 10}, {y, -10, 10},

      VectorScale -> {0.03, Automatic, None},

      VectorStyle -> Opacity[0.3]

    ],

    (* 고정된 점전하 *)

    Graphics[{Red, PointSize[0.02], Point[{0, 0}]}],

    (* 이동하는 점전하 *)

    Graphics[{Blue, PointSize[0.02], Point[{r, 0}]}],

    (* 에너지 레벨 표시 *)

    Graphics[{

      Text[Style["Energy [J]: " <> ToString[ScientificForm[potentialEnergy[r], {5,3}]], 12], {5, 9}]

    }],

    PlotRange -> {{-10, 10}, {-10, 10}},

    Frame -> True,

    FrameLabel -> {"x (m)", "y (m)"},

    PlotLabel -> "Electric Potential Energy"

  ],

  {r, 10, 1, -0.2}

]

  

(* GIF로 내보내기 *)

Export["electric_potential_2d.gif", frames, "AnimationRepetitions" -> Infinity, "DisplayDurations" -> 0.1]
```