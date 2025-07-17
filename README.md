# Practice Kotlin Language on Visual Studio Code

- Kotlin を Visual Studio Code で学ぶ

# コーディング規約

- Kotlin公式が公開しているコーディング規約
    - <https://kotlinlang.org/docs/coding-conventions.html>

#### 1. 命名規則

- クラス・オブジェクト名: UpperCamelCase
- 関数・プロパティ名: lowerCamelCase
- 定数: UPPER_SNAKE_CASE
- パッケージ名: 全て小文字、アンダースコアなし

#### 2. インデント

- スペース4つ（タブではなくスペース）

#### 3. 行の長さ

- 最大100文字

#### 4. 中括弧

- 中括弧は常に同じ行に書き、改行しない:

```kotlin
if (x > 0) {
    println(x)
}
```

#### 5. 空白

- ,, :, =, ->, . などの後にスペース
- : の前にスペースを入れない（型指定時）

```kotlin
val name: String = "foo"
```

#### 6. 関数宣言

- 戻り値が Unit の場合、戻り値は省略

```kotlin
fun foo() {
    // do something
}
```

#### 7. プロパティのアクセサ

- 一行の場合はブロック {} を省略

```kotlin
val isEmpty: Boolean get() = size == 0
```

#### 8. クラスの継承

- : のあとに改行し、インデントを入れる

```kotlin
class MyClass :
    BaseClass(),
    Interface1,
    Interface2
```

#### 9. コメント

- // で単一行コメント
- /**/ で複数行コメント
- KDoc 形式: /** */

#### 10. インポート

- ワイルドカードのインポートは禁止

```kotlin
// 禁止
import foo.*
// 許可
import foo.Bar
```

#### 11. Nullable型

- 明示的に ? を付与する:

```kotlin
val name: String? = null
```
