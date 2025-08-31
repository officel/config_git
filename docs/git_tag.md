# git tag

## 一覧／表示

```bash
# ローカルのタグ一覧
git tag

# -l / --list でフィルタリング
git tag -l "v*"

# リモートのタグ一覧
git ls-remote --tags

# ref も見る
git show-ref --tags

# 個別表示
git show v0.0.0
```

## 作成

```bash
# ローカルの現在のコミットにタグ
git tag v0.0.0

# アノテーションとメッセージをつける
git tag -a v0.0.0 -m 'my version 0.0.0'

# 特定のコミットにつけることもできる
git tag -a v0.0.0 -m 'my version 0.0.0' <commit>
```

## タグの共有

```bash
# ローカルのタグをリモートに送る
git push origin v0.0.0

git push --tags
git pull --tags

# 同名のタグがある場合は上書きでリモートから取得する
git fetch --tags --force
```

## タグを削除

```bash
# ローカルのタグを削除
git tag -d v0.0.0

# まとめて全部消せる
git tag -d $(git tag -l)

# リモートのタグを削除
git push origin :refs/tags/v0.0.0
```
