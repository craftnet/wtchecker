### PITCHMEのお試しプレゼンです


---

### アニメーションテスト
*私の好きなキャンプ場を紹介します

- 道志の森キャンプ場 |
- 館山フラワーパーク |
- 星の降る森 |
- ふもとっぱらキャンプ場 |

---

### グラフやチャートの表示テスト

<canvas data-chart="radar">


    Month, 1月, 2月, 3月, 4月, 5月, 6月, 7月
    1980, 65, 59, 80, 81, 56, 55, 40
    2017, 28, 48, 40, 19, 86, 27, 90


</canvas>
### グラフだよ1

<canvas data-chart="line">
    Month, 1月, 2月, 3月, 4月, 5月, 6月, 7月
    1980, 65, 59, 80, 81, 56, 55, 40
    2017, 28, 48, 40, 19, 86, 27, 90
</canvas>

---

### グラフだよ2

<canvas data-chart="bar">
    Month, 1月, 2月, 3月, 4月, 5月, 6月, 7月
    1980, 65, 59, 80, 81, 56, 55, 40
    2017, 28, 48, 40, 19, 86, 27, 90
</canvas>

---

### グラフだよ3

<canvas data-chart="pie">
    Month, 1月, 2月, 3月, 4月, 5月, 6月, 7月
    1980, 65, 59, 80, 81, 56, 55, 40
    2017, 28, 48, 40, 19, 86, 27, 90
</canvas>

---

### グラフだよ4

<canvas data-chart="radar">
    Month, 1月, 2月, 3月, 4月, 5月, 6月, 7月
    1980, 65, 59, 80, 81, 56, 55, 40
    2017, 28, 48, 40, 19, 86, 27, 90
</canvas>

---

### コードだよ

```
class DecimalEncoder(json.JSONEncoder):
    def default(self, o):
        if isinstance(o, decimal.Decimal):
            if o % 1 > 0:
                return float(o)
            else:
                return int(o)
        return super(DecimalEncoder, self).default(o)
```
---?gist=2e0598b9e36d9fd3b941e54384d95f06

gistに公開した情報を表示しています。


---
### 指定行だけをハイライト

```
var str1 = 'hello world';
var flag = true;
var result = 10 + 20;


console.log( str1 );
console.log( str2 );
console.log( str3 );
```
@[2](flagに「true」を代入)


---
### おわり
