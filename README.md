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
