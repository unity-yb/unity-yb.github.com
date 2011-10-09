
そして、コルーチンは Update の度に再起動されるチャンスがやってきます。実際に再起動されるかどうかは、 yield の指定によって異なります。例えば単に

    yield;

とすれば、コルーチンは次の Update で再起動されます。

    yield WaitForSeconds(1.5);

とすれば、1.5秒間は再起動無しに放置され、その後の Update で再起動されます。

システム側で行なっていることを擬似コードで表すとすれば、次のようなものになります。

function UpdateGameObject ( gameObject )
  for coroutine in gameObject do
    if coroutine.前回のyield返値 != null then
      if not 時間経過チェック( coroutine.前回のyield返値 ) then
        continue // 再起動せずに次へ
    再起動( coroutine )
    if 終了チェック( coroutine ) then
      remove coroutine from gameObject

## コルーチンの素＝イテレーター







## 実は「コルーチン＝イテレーター」

Unityにおけるコルーチンの実体を正確に把握するには、まずこのことを明らかにしておかなければいけません。

