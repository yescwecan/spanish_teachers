# 高校スペイン語教師の会 公式ホームページ

GitHub Pages + Jekyll を前提にした試作版です。

## 現在の内容
- ホーム
- 高校スペイン語教師の会とは
- お知らせ
- イベント
- 入会・お問い合わせ
- プライバシーポリシー
- 404ページ

## ローカル確認の例

Ruby と Bundler が使える環境で、次の流れで確認できます。

1. `bundle install`
2. `bundle exec jekyll serve`
3. ブラウザで `http://127.0.0.1:4000/` を開く

## 補足
- お知らせは `_posts/` に追加します
- イベントは `_events/` に追加します
- 固定ページはルート直下の Markdown / HTML ファイルで管理しています

## GitHub ブラウザからの更新方法

ローカル環境を使わず、GitHub のブラウザ上から本文を更新できます。

### お知らせを追加する

1. GitHub で `_posts/` フォルダを開く
2. `Add file` → `Create new file` を選ぶ
3. ファイル名を `YYYY-MM-DD-article-name.md` 形式で入力する
4. `templates/news-post-template.md` の内容を貼り付けて編集する
5. `Commit changes...` で main に反映する

例: `2026-03-07-spring-workshop.md`

### イベントを追加する

1. GitHub で `_events/` フォルダを開く
2. `Add file` → `Create new file` を選ぶ
3. ファイル名を `event-name.md` 形式で入力する
4. `templates/event-template.md` の内容を貼り付けて編集する
5. `Commit changes...` で main に反映する

例: `2026-spring-meetup.md`

### 文章だけ修正したいとき

- `about.md`: 会の紹介
- `join-contact.md`: 入会・お問い合わせ
- `privacy.md`: プライバシーポリシー

これらは各ファイルを開いて、鉛筆アイコンからそのまま編集できます。

### 注意点

- お知らせはファイル名の先頭の日付で並び順が決まります
- 先頭の `---` で囲まれた設定部分は消さないでください
- 反映後は GitHub Pages の再ビルドに数十秒から数分かかることがあります
