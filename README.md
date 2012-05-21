cmake補助具
========

 * まだ公開できるレベルでない
 * mac下でのみしか動作を確認してない  
 * そもそも俺以外が有用性を見いだせるのか分からない

という三重苦ですが、公開する必要が出てきたためアップします.  
以下このプログラムの精一杯のメリット
 
主な用途
--------
#### ビルド
	cmake_wrapper build

buildディレクトリ作ってそこにcdして`cmake ..`とかやってらんないよ!勝手にやるよ!

#### ビルドして実行
	cmake_wrapper all

ビルドして、buildディレクトリ下にできあがった実行できそうなものを適当に実行するよ!

#### release
	cmake_wrapper init --release && cmake_wrapper build
	
リリースビルドもワンライナーだよ! いちいち`-D CMAKE_BUILD_TYPE=Release`とかめんどくさいよ!

#### CMakeLists.txtを書き換えた後の作り直し
	
	cmake_wrapper reboot
1秒だよ!

#### xcodeとclangの切り替え
	
xcode:
	
	cmake_wrapper reboot --xcode
	
clang:

	cmake_wrapper reboot --clang
	
xcodeでビルドした10秒後にclangでビルドできるよ！

