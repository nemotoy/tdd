# tdd
writes Test-Driven Development

1. テストを書く
2. コンパイラを通す
3. テストを走らせ、失敗を確認する
4. テストを通す
5. 重複を排除する

十分な量のテストがない場合は、あるべきテストを描いてからリファクタリングを行う。

## Part1

### TODO

- [x] $5 + 10 CHF = $10
- [x] $5 + $5 = $10
- [x] $5 + $5がMoneyを返す
- [x] Bank.reduce(Money)
- [x] Moneyを変換して換算を行う
- [x] Reduce(Bank, String)
- [x] Sum.plus
- [x] Expression.times

- [x] $5 * 2 = $10
- [x] amountをprivateにする
- [x] Dollarの副作用
- [ ] Moneyの丸め処理
- [x] equals()
- [ ] hashCode()
- [ ] nullとの比較
- [ ] 他オブジェクトとの比較
- [x] 5 CHF * 2 = 10 CHF
- [x] DollarとFrancの重複
- [x] equalsの一般化
- [x] timesの一般化
- [x] FrancとDollarを比較する
- [x] 通貨の概念
- [x] testFrancMultiplicationを削除する？

## Part2

### TODO

- [x] テストメソッドを呼び出す
- [ ] setUp を最初に呼び出す
- [ ] tearDown を後で呼び出す
- [ ] テストメソッドを失敗したとしても tearDown を呼び出す
- [ ] 収集したテスト結果を出力する

## Part3

* 「テストする」とはどのような意味か？ - ここでの「テスト」とは「自動テスト」(自動で走らせることのできるテストコード群)を言い、コードの変更により何かを壊してしまっているかもしれないストレスを軽減する為にも有用である。
* 何をテストするべきか？ - 実装したいもの。TODOリスト化する。
    * 実装しなければならない振る舞いを列挙する
    * 実装がない操作に関しての空実装をリストに追加する
    * リファクタリングするべき箇所をリストに追加する
* いつテストするか？ - テスト対象のコードを書く前。
    * 設計やスコープ制御の為にも利用できる
    * ストレスを減らせる
* いつアサーションを書くべきか？ - 最初に書く。機能の所属、名前付け、テストの網羅性などをテストを書く際に考える問題は多いので、「正しい結果とは何か？」「どのように検証するか？」の問題を切り離すことでシンプルに考えられる。
* テストデータをどう選ぶか？ - テストを読みやすく、理解しやすくするデータを使う。
    * 取り扱うデータに違いがあるならば意味あるものを利用する
    * 複数のインプットを扱えなければならないのであれば、複数のインプットをテストで実施しなければならない
    * 同じ値は1つのものを表すためだけに利用する(`plus`するだけのメソッドのインプットであれば、1+1ではなく、3+4でテストするといった具合)
* データの意図をどのように示したら良いか？ - 期待値と結果をテスト自身に含め、それらの関係が明確にわかるようにする。
