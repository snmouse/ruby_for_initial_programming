#第2回
-----
##1. 前回の宿題
###Q.下記の文を出力するプログラムを1行かつprint関数を使って書きなさい
	"Hello"
	"World"

###A. 
	print "\"Hello\"\n\"World\""

###解説.
"(ダブルクォーテーション)のようにプログラム言語で使われている文字列を表示する場合、文字列の前に\(バックスラッシュ)を
使うことで表示することができる。このことをプログラミングの世界では「文字列をエスケープする」と言う。
\は、他にも改行やASCII文字を表示するためにも使うことができる。

参考: [http://www.rubylife.jp/ini/string/index2.html](http://www.rubylife.jp/ini/string/index2.html)

ASCII文字とは、標準的な文字列（英数字や記号）のことをいう。

参考: [http://e-words.jp/p/r-ascii.html](http://e-words.jp/p/r-ascii.html)

プログラミングの世界では、文字１つ１つに番号が付けられており、C言語などの低級言語などでは、文字判定にASCII番号を使うこともある。

##2. 講座
ドットインストール　4講座目　[http://dotinstall.com/lessons/basic_ruby/4704](http://dotinstall.com/lessons/basic_ruby/4704)

###補足 1.
ビデオの解説の中では、変数とは値にラベルをつけるものだという解説があったが、
別の考えて変数とは値を入れる箱であるという考え方もある。
変数は、入れる値を変更ができる蓋が空いた箱で、定数は、値を変更できない蓋が閉じた箱である。
定数はどのような時につかうか？それは、円周率などの決まった数字をプログラム中で使うときである。

	例： M_PI = 3.14

ちなみに定数を変更しようとすると、プログラムがエラーを起こし終了する

###補足 2.
これまでは、値をプログラム中に書いていたが、動的に値を変更したいという時もある。
そのときに使うのは、getsという関数である。
たとえば、下記は画面にちょっぴり恥ずかしくなるような文字を表示してくれるプログラムである。

	puts "Please enter your name"
	name = gets
	print "I love "
	print name

このように、getsはキーボードの入力を（改行まで）取得するための関数である。
すでに学んでいるputsは画面に出力する関数であるが、一般的に

**キーボードからの入力のことをSTDIN(Standard Input)**  
**画面への出力のことをSTDOUT(Standard Output)**

という。

###3. 次回までの宿題
出来る範囲でやってきて下さい。

1. getsは改行を含めた値を取得する関数であるが、改行を除くにはどうしたらよいか調べなさい。

2. 下記のプログラムは、入力された値に二倍した値を出力しようとするプログラムであるが、どうもうまくいかない。。。
どうしたらよいかな？

		ptus "Please enter number."
		x = gets
		y = x * 2
		puts y