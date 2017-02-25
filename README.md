# Jupyter notebook 開発環境　セットアップ　手順
## 流れ
1. Homebrewのインストール
2. python環境のインストール（Anaconda）
3. 仮想環境のインストール（conda）
4. 必要モジュールのインストール
5. サンプルコードのインストール
6. jupyter notebookの起動・実行

## 1. Homebrewのインストール
### Homebrewとは？
~~~
「Mac OS Xオペレーティングシステム上でソフトウェアの導入を単純化するパッケージ管理システムのひとつである」
~~~

公式HP：https://brew.sh/index_ja.html

### インストール方法
ターミナルで以下を実行。

~~~bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
~~~

#### ついてにpipもダウンロードしておきます。
ターミナルで以下を実行。

~~~bash
easy_install pip
~~~

参考URL：http://www.task-notes.com/entry/20150810/1439175600

## 2. python環境のインストール（Anaconda）
### Anacondaとは？
~~~
Anaconda は、Continuum Analytics 社によって提供されている、Python 本体に加え、科学技術、数学、エンジニアリング、データ分析など、よく利用される Python パッケージ（2016 年 2 月時点で 400 以上）を一括でインストール可能にしたパッケージです。面倒なセットアップ作業が効率よく行えるため、Python 開発者の間で広く利用されています。なお、Anaconda は商用目的にも利用可能です。
~~~

公式HP：https://www.continuum.io/downloads



以下の記事に沿ってインストールをしていきます。
### 「Anaconda で Python 環境をインストールする」
http://qiita.com/t2y/items/2a3eb58103e85d8064b6

## 3. 仮想環境のインストール（conda）
以下の記事に沿ってインストールをしていきます。
http://qiita.com/supersaiakujin/items/50def6f33b79f9a61b18


#### 発生したエラー（pythonで何かしら開発経験がある人はなる可能性あり）

~~~error
usage: grep [-abcDEFGHhIiJLlmnOoqRSsUVvwxZ] [-A num] [-B num] [-C[num]]
	[-e pattern] [-f file] [--binary-files=value] [--color=when]
	[--context[=num]] [--directories=action] [--label] [--line-buffered]
	[--null] [pattern] [file ...]
pyenv: -bash: command not found

[プロセスが完了しました]
~~~

※　condaとpyenvのactivate衝突エラー回避法
http://baikichiz.hatenablog.com/entry/2017/01/06/163942




## 4. 必要モジュールのインストール
~~~bash
pip install chainer
pip install scikit-learn
pip install matplotlib
pip install jupyter
~~~

## 5. サンプルコードのインストール
もし、gitをインストールしてない場合

~~~bash
brew install git
~~~

~~~bash
git clone git@github.com:tsuruchan/chainer.git
cd chainer
~~~

## 6. jupyter notebookの起動・実行
~~~bash
jupyter notebook
~~~
以下のような画面が表示される。

![スクリーンショット 2017-02-25 18.52.08.png](https://qiita-image-store.s3.amazonaws.com/0/83641/e27d1493-bc74-06bf-2481-a37e49345c75.png "スクリーンショット 2017-02-25 18.52.08.png")


「chainer_mnist.ipynb」をクリックすると以下の画面が表示されます。

![スクリーンショット 2017-02-25 18.52.22.png](https://qiita-image-store.s3.amazonaws.com/0/83641/acdee9ba-5382-27eb-b1a7-16593e7cbd49.png "スクリーンショット 2017-02-25 18.52.22.png")




