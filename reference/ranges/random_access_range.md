# random_access_range
* ranges[meta header]
* concept[meta id-type]
* std::ranges[meta namespace]
* cpp20[meta cpp]

```cpp
namespace std::ranges {
  template<class T>
  concept random_access_range = bidirectional_range<T> && random_access_iterator<iterator_t<T>>;
}
```
* bidirectional_range[link bidirectional_range.md]
* random_access_iterator[link /reference/iterator/random_access_iterator.md]
* iterator_t[link iterator_t.md]

## 概要
`random_access_range`は、イテレータが[`random_access_iterator`](/reference/iterator/random_access_iterator.md)である範囲を表すコンセプトである。

## モデル
型`T`が`random_access_range`のモデルとなるのは、`T`が[`bidirectional_range`](bidirectional_range.md)のモデルであり、かつそのイテレータが[`random_access_iterator`](/reference/iterator/random_access_iterator.md)のモデルである場合である。

## 例
(執筆中)

### 出力
(執筆中)

## バージョン
### 言語
- C++20

### 処理系
- [Clang](/implementation.md#clang): 13.0.0
- [GCC](/implementation.md#gcc): 10.1.0
- [ICC](/implementation.md#icc): ??
- [Visual C++](/implementation.md#visual_cpp): 2019 Update 10

## 参照
- [N4861 24 Ranges library](https://timsong-cpp.github.io/cppwp/n4861/ranges)
- [C++20 ranges](https://techbookfest.org/product/5134506308665344)