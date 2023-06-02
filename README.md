# MathWorks Minidrone Competition
MATLAB主催のドローンコンテストに参加した際のプログラムです．

## 概要
大まかなプログラムは組まれた状態から Flight Control System内のImage Processing SystemとControl Systemを作成しました．

3人1組で開発を行い，私が担当した部分は，
- 円検知時の制御
- PIDの算出

以外の部分です．

開発にはGitを用いていないため完成品のみコミットした状態になっています．

## システム
Flight Control System部でまず得られた画像から赤色のみを1とします．

その後は画面を4分割し，上下，左右の数値変化に対応してControl System部に渡す変数を振り分けます．

４分割の検知とは別に４つ角検知を行い赤い線が直線から曲がったときに対応できるようにしています．