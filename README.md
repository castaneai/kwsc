kwsc
=======
UWSCのちょっとした補助モジュール集

対応UWSCバージョン
----------------------
ver5.0.2（2014/08/11時点の最新版）にて動作を確認している．
For-In文を使用しているため，ver5.0は必須．

モジュール一覧
-----------------

Array
----------
配列に関する処理を行う

- Array.append(arr, v)
配列arrの末尾に要素vを追加

- Array.remove(arr, v)
配列arr中の値がvのものを削除する

- Array.contains(arr, v)
配列arrにvの値を持つ要素が含まれているかを返す

- Array.sequential_equal(arr1, arr2)
2つの配列arr1, arr2の要素数が同じで，すべての要素が順序どおり同じ値を持つかどうかを返す

Bit
----------
ビット演算を行う

- Bit.lshift(v, n)
値vをn回左シフトする

- Bit.rshift(v, n)
値vをn回右シフトする

Debug
-----------
printデバッグを支援

- Debug.print_array(arr)
配列arrを見やすく表示する

- Debug.print_2d_array(arr)
2次元配列arrを見やすく表示する

- Debug.print_hashtbl(tbl)
ハッシュテーブル（連想配列）tblを見やすく表示する

Dist
-----------
スクリプト配布支援

- Dist.build(src_files, dst_file)
対象のuwsスクリプトファイルパスの配列src_filesを読み込み，
結合してスクランブルを施し1つのuwsファイルパスdst_fileに保存する

* Hex: 16進数文字列操作
* Ini: iniファイルの読み書き
* Input: マウス/キーボード入力
* Profiler: 処理時間計測
* Socket: TCPソケット処理
* Test: テスト
* Window: ウィンドウ制御