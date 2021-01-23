# Rils Girls
---
## 参考資料

- rails　インストール時のエラー
  https://qiita.com/NaokiIshimura/items/8203f74f8dfd5f6b87a0
- rails girls
  https://railsgirls.jp/app
- rails install
  https://zenn.dev/s7/articles/b3252543eab33a65052a

---

1. 新しいアプリの作成
```
 $ rails new rails-girls
 $ cd rails-girls 
 $ rails server
 ```

※errorが出る or うまく動かない時

- webpackがインストールされていない
　bundle installの時点でwebpackがインストールできていないと表示が出る

  - yarnをインストール
    ```
    $ curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
    $ echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
    $ sudo apt-get update && sudo apt-get install yarn
    ```
    インストール確認
    ```
    $ yarn -v
    $ yarn install
    ```

  - nodeがインストールされていない
    ```
    sudo apt install -y nodejs sqlite3 npm
    npm install -g n
    sudo n stable
    exec $SHELL -l
    ```
    インストール確認
    ```
    node -v
    ```

2. 