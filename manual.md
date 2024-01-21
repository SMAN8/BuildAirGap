## インストール要件 ##
### 環境 ###
+ Windows11 Home
+ 実装RAM8.00GB
### ダウンロード/インストール ###
+ Ubuntu 20.04.06 LTS
+ VirtualBox-7.0.12

### ※更新した手順番号 ###
**インストール要件から手順７番まで**

## 1.OS Ubuntuの入手 ##
### 1-1.サイトへ移動したら、下の画像の赤い四角をタップしダウンロードする。 ###
[UbuntuディスクのDL先のサイトへ移動](https://releases.ubuntu.com/20.04/)
> ダウンロードする際、少し時間がかかります。
<img width="1011" alt="1：2023-12-26 112310" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/0ca315a9-176f-45fe-a600-f55f80a12ab3">

### 1-2.UbuntuディスクISOの保存場所の作成 ###
+ VirtualBoxをインストールした際に作成されるユーザーフォルダ内の「VirtualBoxVMs」フォルダ内に保存。
> VirtualBoxのインストールが完了するまではUbuntuディスクを一旦ダウンロードフォルダに入れて置いて、インストールが完了してから移動する。今ここで移動したとしても問題ないです。

> デフォルトだと「C:\Users\[ユーザー名]\Virtuasudo adduser $USER vboxsflBox VMs」下に仮想マシン名のフォルダが作られます。フォルダが作成されていなければ、新たにフォルダを作成して下さい。
<img width="880" alt="２：　　　　 2024-01-05 134933" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/0a3c0d02-1c10-4989-8dde-402c4238cce2">

## 2.VirtualBoxのダウンロード ##
### 2-1.VirtualBoxのダウンロードサイトへ移動し`Windows hosts`をタップする。 ###
[ここをタップすると、VirtualBoxのDLサイトへ移動します](https://www.virtualbox.org/wiki/Downloads)

<img width="1010" alt="４： 2023-12-26 130426" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/abf74833-ac1d-4314-ad82-29700b068659">

## 3.VirtualBoxのインストール ##
### 3-1.ダウンロードしたVirtualBoxのインストーラーをダブルクリックする。 ###
<img width="877" alt="５： 2023-12-26 210724" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/1b7ef9cd-6445-46f5-9cf5-0b41c6b9e615">

### 3-2.この画面になったら`NEXT>`を押す ###
<img width="384" alt="６： 2023-12-26 204112" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/cf5b9431-73c5-489c-ae52-aeb66ae9aba6">

### 3-3.続けてそのまま`Next>`、`Yes`をタップして行き、最後に`Install`をタップ ###
![７：4工程纏め](https://github.com/SMAN8/Create-of-AirGap/assets/80440848/950220df-b900-40d0-9a7c-2175e3018f31)

### 3-4.Windowsセキュリティが作動し、デバイスのソフトウェアをインストールしますか？と聞かれたら`インストール(I)`をタップし、下の画像の赤い四角で囲まれた`Finish`をタップする。
<img width="385" alt="８： 2023-12-26 204404" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/646136ca-530b-4cdf-b3a5-88b97b9617ef">

### 3-5.VirtualBoxの管理画面が立ち上がり、インストールが完了しました。 ###
<img width="959" alt="９： 　　　　2023-12-26 204428 " src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/bdbf8f90-2dae-4b6a-844b-069c02cc2e94">

## 4.VirtualBoxの仮想マシンの作成 ##
### 4-1.仮想マシンを作成する為に下の画像の赤い四角の`新規(N)`をタップする。 ###
<img width="959" alt="１０： 2023-12-26 204428" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/3e627022-6213-4f0f-8342-cf9f94988404">

### 4-2.仮想マシンの名前とOSの設定 ###
+ 名　　前  ・・・任意の仮想マシン名（下の例：AirGap)
+ フォルダ  ・・・仮想マシンの生成されるファイルを保存する場所を指定する
+ ISO Image・・・1-2に保存したUbuntu-ISOファイルを指定する
+ 「自動インストールをスキップ(S)」にチェックして `次へ`  をクリック
<img width="816" alt="１１：　　　 2024-01-05 134712" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/f3212e93-4b89-46ca-85b3-98ec77bc4ece">

### 4-3.メモリとコアの設定 ###
+ メインメモリーを`4096MB`に、プロセッサー数を`2`に変更する
<img width="815" alt="１２：　　　 2024-01-06 200017" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/c5e3397c-cecb-4347-a757-5a4d285bf270">

### 4-4.仮想マシンのハードディスクのサイズ設定 ###
+ ディスクサイズを`50.00GB`に変更し、`次へ(N)`をタップ
<img width="816" alt="１３：　　　 2024-01-04 184025" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/d3d316ff-9966-48d4-86b9-f666f32c533a">

### 4-5.VirtualBoxの仮想マシンの作成完了 ###
+ 概要を確認して、問題がなければ`完了(F)`をタップして完了
<img width="819" alt="１４：　　　 2024-01-05 140646" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/a4c444c3-a846-461a-99e1-a620a428b41f">

## 5.仮想マシンの環境設定 ##
### 5-1.使用する仮想マシン（ここではAirGap）を選択し、「設定」アイコンをタップする ###
<img width="895" alt="１５：2024-01-20" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/ec85a7e2-02b9-4a27-a85f-9c06cadd17f4">

### 5-2.一般 ###
+ 「一般」→「高度」タブから**クリップボードの共有**と**ドラッグ＆ドロップ**を`「双方向」`に変更してOKをクリック
<img width="774" alt="１６：　　　 2024-01-04 202541" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/ed2b8e9f-452f-4206-b21b-9fb6daa01dd7">

### 5-3.システム ###
+ 「システム」→「マザーボード」タブの**フロッピー**の`チェックを外す`・**チップセット**を`ICH9に変更`してOKをクリック
<img width="772" alt="１７：　　　 2024-01-06 183847" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/b7aec409-438a-442c-87e4-f357799bcbbf">

### 5-4.共有フォルダの作成 ###
+ WindowsとUbuntu間の**共有フォルダ**(ここではShare)を作成する（ドキュメントフォルダなどの任意の場所）
> 共有フォルダを作成する際にフォルダの階層が深すぎると共有化できない場合があるので、階層を変えて作成してみてください。
<img width="880" alt="１８：　　　 2024-01-06 141528" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/0220b62c-f1f4-445c-a0b4-a723ef69c5e5">

### 5-5.仮想マシンから共有フォルダを指定選択する ###
+ 「フォルダーパス」に５-４で作成したフォルダを指定する
+ マウントポイントに`/media/share_win`を入力する
+ `自動マウント`にチェックする

![１９：　　　 2024-01-04 205659](https://github.com/SMAN8/Create-of-AirGap/assets/80440848/bce463bf-0e98-4b4e-8a80-eb6a5dd2d54f)

<img width="773" alt="２０：　　　 2024-01-04 204745" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/132c888d-2a5a-4f24-98ec-4126bb7f96d5">

## 6.Ubuntuのインストール ##
### 6-1.作成した仮想マシンの`起動`をクリック ###

<img width="891" alt="２１：　　　 2024-01-20 123433" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/6ebe345e-d1bc-44d1-a1d9-311613d556e9">

### 6-2.下の画像のようにディスクが`起動`し始めます。 ###

<img width="398" alt="２２：　　　 2024-01-05 144534" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/3b1b048e-0226-4877-be45-aae1761ad424">

### 6-3.左の枠の中から日本語を選択します ###

<img width="399" alt="２３：　　　 2024-01-05 151918" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/e8ea03c3-9906-4f77-b072-bbc3b7f6112a">

### 6-4.日本語に変換されますので、下の画像の赤い四角の`Ubuntuをインストール`をタップします。 ###

<img width="400" alt="２４：　　　 2024-01-05 151429" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/d7da031c-fbb2-4639-8d07-6785f2180e9c">

### 6-5.日本語キーボードの方は、両方とも`Japanese`を選択し、設定が完了したら`続ける`をクリックします。 ###
> USキーボードの方は「キーボードレイアウト」→「キーボードレイアウトの検出」をクリックして設定してください。※**画面が見切れている場合**の対処法：`Alt + F7を押す`とマウスでウィンドウを移動できます。

<img width="519" alt="２５：　　　 2024-01-05 160005" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/1d232a63-9693-4ab9-bc1d-d41b6c7dbae5">

### 6-6. 下の画像の状態のまま、`続ける`をタップ

<img width="518" alt="２６：　　　 2024-01-05 160756" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/a24ccaea-cdc0-4470-aa21-1e6c7f1847b9">

### 6-7.下の画像の状態のまま、`インストール`をタップ ###

<img width="519" alt="２７：　　　 2024-01-05 161209" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/948234e0-a9e6-4011-9671-efc70cc7e0e3">

### 6-8.`続ける`をタップ ###

<img width="518" alt="２８：　　　 2024-01-05 161509" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/b004bad5-2cab-4c36-b92d-90c696d2848d">

### 6-9.お住まいの地域をクリックし、`続ける`をクリック

<img width="518" alt="２９：　　　 2024-01-05 161806" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/16fc8916-9e2e-4bbd-a884-9512e3df9009">

### 6-10.`あなたの名前`はマシン名を入れると、その下の`コンピューターの名前`、`ユーザー名`の入力にも自動で入力されます。そして、パスワードをご自身で決めて入力を済ませて下さい。終わりましたら、`続ける`をタップ。

<img width="519" alt="３０：　　　 2024-01-05 162408" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/962d1e99-c1f0-4d45-8d04-6d0b41c57e6f">

### 6-11.Ubuntuのインストールが始まりました。暫くお待ち下さい。 ###

<img width="518" alt="３１：　　　 2024-01-05 162845" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/4d679f01-7da7-4b1c-b9ca-0c5b4e8d25d4">

### 6-12.インストール完了後、`再起動`をタップ

<img width="518" alt="３２：　　　 2024-01-05 163835" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/be65093f-7fdb-48a0-b319-5ea1b10f7d74">

### 6-13.ログイン ###
+ キーボードのENTERボタンを押します

<img width="520" alt="３３：　　　 2024-01-05 164133" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/205854d1-aecc-4aee-a79f-71bd8786ca98">

+ 6-10.で登録した**パスワード**を入力しログインします

<img width="520" alt="３４：　　　 2024-01-05 164520" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/7223a33c-e8f2-4aa3-abad-05ad0a92a1cb">

### 6-14.オンラインアカウントの接続は、右上の`スキップ(S)`をクリック ###

<img width="517" alt="３５：　　　 2024-01-05 164718" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/0eb8fbef-78ad-4ef7-b711-fd08abea8259">

### 6-15.`次へ`をタップします

<img width="519" alt="３６：　　　 2024-01-05 165506" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/33176e47-042e-45c4-b562-3b16613d37e4">

### 6-16.`いいえ、送信しません`を選択し、右上の`次へ(N)`をタップ ###

<img width="520" alt="３７：　　　 2024-01-05 165922" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/6953e784-79c2-47df-b15f-6b5e9f962d7c">

### 6-17.そのまま、`次へ(N)`をタップ ###

<img width="519" alt="３８：　　　 2024-01-05 170311" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/81772521-02e1-4df7-901e-861d7bd98d42">

### 6-18.インストールが終わりました。`完了`をクリック ###

<img width="519" alt="３９：　　　 2024-01-05 170521" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/e53c0866-4b4e-41a5-9b48-8980bafc5a3c">

### 6-19.Ubuntu新バージョンは`アップグレードしない`をクリック ###

<img width="520" alt="４０：　　　 2024-01-05 170847" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/4129feec-385b-4c4d-9344-bdcf1e9f77c2">

### 6-20.`OK`をクリック ###

<img width="519" alt="４１：　　　 2024-01-05 171157" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/e60467b0-fdd6-4519-874f-952f3333f293">

### 6-21.`この操作を今すぐ実行`をクリック ###

<img width="518" alt="４２：　　　 2024-01-05 171555" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/2b5690f8-847b-4213-9c1d-7db0da3a12f0">

### 6-22.`インストール`をクリック

<img width="520" alt="４３：　　　 2024-01-05 171745" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/47f7e82a-f4ff-4065-b6ab-57077c556258">

### 6-23.パスワードを入力し、`認証`をタップ ###

<img width="519" alt="４４：　　　 2024-01-05 172012" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/cdabbc06-18df-4549-a326-6ba64da891b9">

### 6-24.しばらく変更の適用が完了するまで待ちます。 ###

<img width="519" alt="４５：　　　 2024-01-05 172348" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/684a4161-a7c8-47da-b3dd-162d850c2ae0">

### 6-25.インストール完了後、`全体に適用する`をクリックし閉じる ###

![４６：　　　 2024-01-05 183911](https://github.com/SMAN8/Create-of-AirGap/assets/80440848/ce7d8d2d-7f41-4fae-b04b-976b699a0463)

## 7.Guest Additionsのインストール ##
+ アプリ一覧からターミナル(端末)を起動し以下コマンドを手動入力する。

```
sudo apt update -y
sudo apt upgrade -y
sudo apt install gcc make perl -y
```

> まだコピーアンドペーストが利用できない為、タイプミスに留意して下さい。

### 7-1.ホストメイン画面上部の`デバイス`タブから`Guest Additions CDイメージの挿入…`をタップします。 ###

<img width="519" alt="４７：　　　 2024-01-05 190705" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/40550769-f022-4c8e-a10c-5b98e5a0dd9d">

### 7-2.以下のメッセージが表示されたら`実行(R)`をクリックした後、パスワードを入力し、`認証ボタン`をタップします。

<img width="518" alt="４８：　　　 2024-01-05 191029" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/15b78338-b7f9-4a5f-9aad-d7b80be207fc">

### 7-3.下の画像内の赤いラインのように処理完了のメッセージが表示されましたら、`Enter`キーをタップします。

<img width="518" alt="４９：　　　 2024-01-05 191712" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/bdf95e54-5a58-45a5-9cb8-1e924a83ee79">

### 7-4.ターミナル(端末)を起動しユーザーをグループ化するコマンドを実行 ###

> 左上のアクティビティをタップします。そして検索窓にterminalの`t`と入れると下の画像のように端末が表示されます。

<img width="519" alt="５０：　　　 2024-01-05 201746" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/99d7f0a0-6861-4a0d-805a-c2246c47df6b">

> 端末をタップし、起動させユーザーをグループ化するコマンドを実行

```
sudo adduser $USER vboxsf
```

<img width="520" alt="５１：　　　 2024-01-05 202410" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/8d75aba5-f011-46dc-8bcb-b034403c9a9b">

> 下の画像のようにユーザーがグループ化された事を端末で確認できます

<img width="518" alt="５２：　　　 2024-01-05 202644" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/6c56cfba-237a-4558-8a05-db9aeb1620bd">

### 7-5.フォルダに`share_win`が表示されていれば、5-5.の「共有フォルダ」で設定したローカルPCのフォルダと同期します。 ###

<img width="519" alt="５３：　　　 2024-01-05 203211" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/9d90b7c4-3288-455b-9530-4d03b1c8a897">

### 7-6.コピー＆ペーストできるか`ホストPC`でテキスト文字をコピーして`ゲストOS`の端末で右クリックして貼り付けしてみる。
> メモ帳にコピー用として`aiueo`と入力し、`Ctrl + A`で全選択→`Ctrl + C`でコピーする

<img width="649" alt="５４：　　　 2024-01-06 185300" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/658ef1ca-69a2-40c3-b12d-b2c18c5fa7c8">

+ 仮想マシンのUbuntuOS内の端末に`Ctrl + V`でペーストする。ペーストできたら、OKです。

+ もし、コピー＆ペーストできなかった場合は、下の対処方法を行ってみてください。

<img width="398" alt="５５：　　　 2024-01-06 185826" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/0fa41760-1f2e-4c25-b830-746925204e5c">

### コピー＆ペーストが出来なかった場合の対処方法 ###
+ 端末を開き、右上の`ハンバーガーボタン`をタップし、`設定(P)`をタップする

<img width="401" alt="５６：　　　 2024-01-06 185107" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/fdd16f50-4688-4c95-b9ad-e757c30b3633">

+ `ショートカットタブ`をタップし、編集の中の`コピーと貼り付け`のショートカットを確認。
+ コピーのショートカットが、`Shift + Ctrl + C`、貼り付けのショートカットが`Shift + Ctrl + V`になっている場合があります。ローカルPCのショートカットと一緒に変更しておくと、楽なので、それぞれコピーと貼り付けを`Ctrl + C`と`Ctrl + V`に変更しておきます。
+ それぞれのショートカットキーを変更したら、端末でコピー＆ペーストを試してみてください。

<img width="476" alt="５７：　　　 2024-01-06 191013" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/3038e42f-768c-439c-9626-c5c2c9703d96">

### 7-7.表示→ゲストOSの画面を自動リサイズにチェックが入っている事を確認します。
+ チェックが入っていなければ、チェックを入れて下さい。

<img width="475" alt="５８：　　　 2024-01-06 192216" src="https://github.com/SMAN8/Create-of-AirGap/assets/80440848/1f60c434-17a5-4e10-8dae-cd0ddb488f8e">

+ 上記手順を行っても、「共有フォルダが表示されない」「共有フォルダ化されていない」場合は、一度VBox_GAs_7.0.12をアンマンウントしてから再度挿入し、再起動すると共有フォルダは完了します。それでもダメなら[GUI操作でGuest Additionsがインストールできなかった場合](https://docs.spojapanguild.net/setup/air-gap-guid/#6-swap)を試してください。
