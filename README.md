# Hello World チュートリアル

codecheckへようこそ！  
ここではcodecheckの試験の受験方法を簡単に紹介いたします。  
まずは緑色のボタンを押し、チャレンジを開始してください。

## 1. codecheckで「Hello world」を試してみよう

### 1-1.  制限時間・締切を確認しよう
画面上部に、制限時間・あるいは解答締切が表示されるようになります。  
制限時間や締切をオーバーすると解答の提出ができませんので、ご注意ください。  
![制限時間の表示](images/time_limit.png)

### 1-2. Webエディタ or GitHubでの解答の選択
codecheckでは専用のWebエディタで問題を回答するか、  
チャレンジによってはGitHubアカウントを活用して、自身のローカル環境にて問題の回答をすることが出来ます。  
**まずは、画面右側にある"Webエディタで開く"ボタンをクリックして、Webエディタを立ち上げてみましょう。**  
!["Webエディタで開く"ボタン](images/open_challenge_buttons.png)

---

## 2. Webエディタで解答してみよう

### 2-1. ファイルを開く
Webエディタをひらいたら、[こちらのリンク](test/basic.js)をクリックしてください。  

リンクで指定されたファイルが、エディタ上で開かれていることを確認してください。  
リンクをクリックして指定されたファイルを表示することが可能です。  
同じく、Webエディタ上の画面左側のプロジェクトツリーからもファイルをクリックして開くことが可能です。

### 2-2. 要求内容の確認
以下のようにチャレンジの要求している内容が問題文の中で紹介されます。  
要求内容を熟読した上で実装をすることをお勧めします:

```
ザ・ミッション:
今回は"World"が入力された時、"Hello World!"と返し、  
"codecheck"の場合は、"Hello codecheck!"と返すような関数を実装してください。
```

### 2-3. ファイルの編集
Webエディタ上のファイルを編集してみましょう。  
[answer.md](answer.md)を開き、`## Q1. 得意なプログラミング言語`  と表記してある下の行に自分の得意とするプログラミング言語を記入してください。

![answer.mdの編集](images/favorite_programming_lang.png)

### 2-4. ファイルの保存
編集したファイルの実行にはまず編集したファイルの保存が必要です。  
編集が完了したら、画面右上の"保存する"ボタンをクリックしましょう。  
"answer.md"にチェックが入っていることを確認して、ファイルを保存してください。  

![save_files_modal](images/save_files_modal.png)

保存が完了したら"編集を続ける"ボタンを選択しましょう。

### 2-5. ファイルの実行
正しく実装できているかどうかを確かめるために、テスト（正しく動いているかどうかを確かめるコード）を実行することが出来ます。  
エディタ中部の”テスト実行”ボタンをクリックしてみましょう。  
クリックすると、テストコードが実行されます。少々時間がかかりますが、最後に

```
codecheck: Finish 'npm install with code 0
1..2
ok 1 helloWorld Hello World!
# tests 2
# pass 1
# fail 1
codecheck: Finish with code 1
codecheck: tests  : 2
codecheck: success: 1
codecheck: failure: 1
```

と表示されれば問題なく実行されています。  
上記の出力の場合、テストケース（期待される入力と出力値）2つに対して、1つが正しく回答ができている事になります。

### 2-6. 正しい解答をしてみよう
現段階では、完璧な回答ではありません。  
先ほど表示されていた[basic.js](test/basic.js)  
の2つのテストを通過するコードを書いてみましょう。

入力値を引数に取り、期待されている結果を標準出力に出力するCLIアプリケーションとして解答を実装してください。  
CLIの実装方法については[指定言語].md に記載されており、Webエディタの右上のタブから選択できます。  

![CLIの実際方法の記載場所](images/cli_instructions.png)

もし、正しく解答ができた場合は、

```
codecheck: Finish 'npm install with code 0
1..2
ok 1 helloWorld Hello World!
# tests 2
# pass 2
# fail 0
codecheck: Finish with code 1
codecheck: tests  : 2
codecheck: success: 2
codecheck: failure: 0
```
と表示がされます。このように、codecheckでは、テストコードを読みながら、正しく仕様を満たす実装を書くプラクティスをおこなうことが可能です。

### 2-7. 保存されているかの確認
編集が完了したら、改めて画面右上の"保存"ボタンをクリックしましょう。  
編集されたファイルがない場合は、"保存されたファイルはありません"と表示されます)  
表示されているダイアログから、"エディタを閉じる"ボタンをクリックして、チャレンジの詳細画面に戻ってください。  
"Webエディタで開く"ボタンの上に、"保存 on [保存された時間]"が表示されていれば正しく保存ができていることになります。

![保存の確認](images/confirm_saved_2.png)

---

## 3. GitHubを使って解答してみよう（※GitHubユーザ向け）
### 3-1. GitHubアカウントの連携
まず、GitHubを活用して回答をする場合、codecheck内でGitHubアカウントの連携が必要です。  
[こちらのページ](https://app.code-check.io/settings/social)から、GitHubアカウントの連携をおこないます。

![ソーシャルアカウントの連携画面](images/github_integration_2.png)

こちらの「接続」をクリックし、GitHubのアカウントの連携をしてください。  
アカウントの連携が完了しましたら、再度こちらの画面をリロードしてください。  
正しく接続が完了すると、"GitHubで解く"ボタンが選択できるようになります。

### 3-2. チャレンジをフォークしてみましょう
画面右側の"GitHubで解く"をクリックしてみましょう。  

![チャレンジのフォーク画面](images/fork_repo_modal_empty.png)

上記のダイアログが立ち上がったら、リポジトリ名を入力して、作成を選択してみましょう。  
すると、GitHubの生成されたリポジトリURLが表示されます。

![レポジトリの作成に成功しました](images/fork_repo_modal_success.png)

表示されたURLをクリックすると、生成されたGitHubのページにジャンプすることが出来ます。

### 3-3. ファイルの編集
GitHubを使って回答の編集をしてみましょう。  
ローカルにクローンをすれば、自分自身の好きな環境やエディタで自由に回答を編集することも可能です。  
今回は、`answer.md`を編集してみましょう。  

### 3-4. 回答のPush
回答を編集したら、編集内容をcodecheck上に保存します。  
リモートのmasterにプッシュ(`git push origin master`)するだけで、回答内容をcodecheck上に保存する事ができます。  
無事にリモートのmasterにプッシュが完了すると、codecheck側にもmasterの編集内容が保存されます。  
masterにpushした後、チャレンジの詳細画面に戻ってください。  
「保存」の下に表示されている時間が、pushをした時間に切り替わっていれば、正しく保存が完了しています。  

![保存の確認](images/confirm_saved_2.png)

### 3-5. 保存されているかの確認
保存が完了したら、正しく保存ができているのか、改めてWebエディタで確かめてみましょう。  
Webエディタ画面を再度開いてみてください。(既に開いている場合はリロード)  
編集したファイルが正しく保存され、更新されていれば完了です。  
また、画面右上のSAVEボタンが押せなくなっており"READONLY Solving in GitHub"と表示されます。  
**一度GitHubで受験をし、ローカルから保存をすると、Webエディタからは編集・保存ができなくなるので、ご注意下さい**

また、Webエディタ上で`answer.md`を開いてみましょう。
あなたがローカルで編集した内容が反映されたら成功です。  

最後に、テスト実行ボタンを押してみましょう。
```
codecheck: Finish 'npm install with code 0
1..2
ok 1 helloWorld Hello World!
# tests 2
# pass 2
# fail 0
codecheck: Finish with code 0
codecheck: tests  : 2
codecheck: success: 2
codecheck: failure: 0
```

が表示されたら正しく解答ができていることになります。  
このように、GitHub上で受験、保存をした後も、Webエディタ上でテストの結果を確かめることは可能です。

---

## 4. チャレンジを提出しよう
### 4-1. answer.mdの表示とコメント
codecheckでは、あなたが工夫して解答した点を[answer.md](answer.md)にまとめることが出来ます。
こちらのファイルを開いて、コメントアウトに記載されてる質問に回答してみましょう。  
このように、codecheck上では、
- 提出したプロジェクト(リポジトリ、ソースコード)
- 記入したanswer.md
を活用して自身のエンジニアスキルを表現することが可能です。  

### 4-2. チャレンジの提出
全ての解答内容の保存が確認できたら、解答を提出しましょう。
チャレンジの詳細画面に戻り、画面右上の「提出（submit）」ボタンを押して「OK」をクリックすると、提出が完了します。  
一度提出をすると、変更や再受験は出来ませんので、ご注意ください。

---

## 5. その他
### 環境変数の利用について

APIキーや認証トークンなど、**秘匿する必要のある変数は、github上に直接アップロードしないでください。**  
キーを実装物にハードコードしたままgithubにpushしてしまうと、  
個人用のAPIキーなどの情報が公開されてしまい、悪用される可能性が発生します。

代わりに、codecheckの環境変数機能をご利用ください。  
秘匿したい情報をgithub上に公開せずにcodecheck内で利用し、  
正しく動作するコードをcodecheck上に提出することが可能になります。

1. 試験のチャレンジ一覧ページ、チャレンジ横にドロップメニューのボタンが表示されます。  
  ![exam_challenge_list_masked_sm](https://user-images.githubusercontent.com/7766684/31326767-4145f402-ad05-11e7-8f38-fc55913a2776.png)

2. そのボタンをクリックすると、「環境変数の設定」という項目が表示されます。  
 ![triangle_dropdown](https://user-images.githubusercontent.com/7766684/31326777-49570ec4-ad05-11e7-914c-d61b245109dd.png)

3. 「環境変数の設定」をクリックし、任意の命名でAPIキー等の環境変数を設定ください。  
 ![env_modal_sm](https://user-images.githubusercontent.com/7766684/31326778-4b594944-ad05-11e7-949d-b96019e7bc87.png)
