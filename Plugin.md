v2.4.0においてプラグイン機能を更新しました。

`Ched.Plugins`名前空間内のインタフェースを実装することでプラグインを作成できます。

## プラグイン種別

  * `IScorePlugin`
    + 譜面データに対する処理を提供します。

## プラグイン作成

Nugetから`Ched.Plugins`を参照に追加します。

インターフェースを実装したクラスを作成してビルドしたdllファイルをChedの実行フォルダ内に作った`Plugins`フォルダに放り込めば動作します。

## プラグインのサンプル

  * [コンボ計算プラグイン](https://github.com/paralleltree/Ched/blob/develop/Ched/Plugins/ComboCalculator.cs)
  * [Seaurchin仕様コンボ計算プラグイン](https://github.com/paralleltree/Seaurchin/blob/develop/Cheddeaurchin/SeaurchinComboCounter.cs)
