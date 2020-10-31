# evEdit
event editor
```
let eve=evEdit({ctx:ctx,key:key,cash:{} }) //key is ^v<>ABXYLR
eve.add(`#F00X00Y00
＠back.jpg //背景基本はフル
＠＜aaaa.jpg,1.2　//左 scale //等倍で拡大しない。
＠＠aaaa.xyz,1.3 //中央
＠＞rrrr.jjj,1.5 //右
％BGM
％％SE

制御記号以外は文字列。
山田「文字列の中にカギカッコがある場合、名前分、ここでいう山田分、左スペースが生まれる」

？一問一答しかできない。$1
１．あいう|これアイウです。補助。
２．さしす｜これはさしすです。
＊３．せせせ  //first choice
４．こここ


`)

let ask=await eve.run('#F00X00Y00','リプレイス/*$1*/') //不明なアドレスはwarning
//もし設問がある場合は、リターンで番号が還る。
eve.getFlg('#F00X00Y00') //1,2,3

```
