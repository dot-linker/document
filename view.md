

# 画面の作成（View）

1. [Bladeファイルの作成](#blade)
2. [ViewMakerファイルの作成](#viewMaker)

<a name="blade"/>
## Bladeファイルの作成
### 作成場所

```resorce/views``` 以下にある、それぞれのディレクトリ内に作成する。

* ユーザー関連： ```/user```
    * ユーザー設定関連: ```/setting```
    * ユーザーページ関連: ```/page```
* イベント関連: ```/event```
* エラー関連: ```/error```

***命名規則***
ファイル名はアッパーキャメルケース(単語の頭文字を大文字、それ以外は小文字)で
ディレクトリ構造で表現できる単語を除き英語に置き換える

例）ユーザーメール通知設定画面 ```resorce/views/user/setting/MailNotice.blade.php```

***共通ブレードの扱い***
共通部分が存在する場合はその物事でディレクトリを作成し、その直下に ```layout.balde.php``` を作成する

例）ユーザー設定画面 ```user/setting/layout.blade.php```

***コンポーネントの扱い***
関連する物事のディレクトリに ```components``` ディレクトリを作成する。

例）イベントカード　```EventCard.blade.php```

<a name="viewMaker"></a>
# ViewMakerファイルの作成

### ViewMakerとは？
PHPの[タイプヒンティング](http://php.net/manual/ja/language.oop5.typehinting.php)を利用し、コントローラ製作者に必要なデータを知らせるためのクラス

### 作成場所

```app/ViewMaker``` 以下にある、それぞれのディレクトリ内に作成する。

* ユーザー関連： ```/User```
    * ユーザー設定関連: ```/Setting```
    * ユーザーページ関連: ```/Page```
* イベント関連: ```/Event```
* エラー関連: ```/Error```


