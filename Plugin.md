v2.2.0よりプラグイン機能を追加しました。
`Ched.Plugins`名前空間内のインタフェースを実装することでプラグインを作成できます。

## プラグイン種別

  * `IScorePlugin`
    + 譜面データに対する処理を提供します。

## プラグイン作成

プラグイン用のプロジェクトを作成してChedを参照に追加します。
現状DLL分割ができていないので`Ched.exe`を追加する形となります。ゆるして
LocalCopyをFalseにしないと[面倒なこと](https://twitter.com/kb10uy/status/1046007143378300928)になります。

インターフェースを実装したクラスを作成してビルドしたdllファイルをChedの実行フォルダ内に作った`Plugins`フォルダに放り込めば動作するはずです。

## プラグインのサンプル

  * [コンボ計算プラグイン](https://github.com/paralleltree/Ched/blob/develop/Ched/Plugins/ComboCalculator.cs)
  * [Seaurchin仕様コンボ計算プラグイン](https://github.com/paralleltree/Seaurchin/blob/develop/Cheddeaurchin/SeaurchinComboCounter.cs)
