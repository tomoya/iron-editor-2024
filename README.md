# エディタの鉄人 2024

こちらは[東京Emacs勉強会 サマーフェスティバル2024](https://tokyo-emacs.connpass.com/event/321255/)で行われたエディタ鉄人のお題リポジトリです。

## お題1

[東京Emacs勉強会 サマーフェスティバル2024 参加者一覧](https://tokyo-emacs.connpass.com/event/321255/participation/#participants)をコピーして作成したテキスト [source.txt](source.txt)ファイルから、参加者一覧のリストを作成してください。

### 回答例

こんな感じでユーザー名を1行づつにしてください。

```
Kyure_A
yasunori
nekurai
...（以下略）
```

## お題2

[schema.prisma](schema.prisma)ファイルから、以下のtbls用のコメントYMALファイルを作成してください。

```yaml
comments:
  - table: Session
    tableComment: アカウント
    columnComments:
      id: ユーザーID
      userId: ユーザーID
      type: タイプ
      refresh_token: リフレッシュトークン
  -
    table: Session
    tableComment: セッション
    columnComments:
      id: ユーザーID
      sessionToken: セッショントークン
      userId: ユーザーID
      expires: 失効日時
  -
    table: User
    tableComment: ユーザー
    columnComments:
      id: ユーザーID
      name: 名前
      email: Eメール
      emailVerified: 認証済みフラグ
```
