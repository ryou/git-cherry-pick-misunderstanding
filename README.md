# cherry-pickが指定したコミットの差分を適用するものではないと実際に試せる例

`feature` ブランチのコミット `add 2nd line` だけを `master` に適用しようと思って

```
git switch master
git cherry-pick 588e53aac96598d1271248fa128a09364c92daf0
```

としようとすると、 `add 1st line` で追加された行も適用されてしまう、というcherry-pickが差分適用じゃないことが分かる例
