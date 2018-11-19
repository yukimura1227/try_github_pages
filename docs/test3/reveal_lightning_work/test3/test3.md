
<div uk-grid>
<div class="uk-width-1-2">
<ul>
  <li>hoge</li>
  <li>fuga</li>
</ul>
</div>
<div class="uk-width-1-2">
~~fugafuga~~
</div>
</div>

---

### オニオンアーキテクチャ

.Jeffrey Palermo氏が提唱したアーキテクチャ
<br>外側の層から内側の層のみ依存関係

~~{:left}~~

.特徴 :mag:
 - ドメインモデルは完全独立
   * インフラの寿命は３年
 - 依存性逆転の法則(DIP)
   * 内: インタフェースを定義
   * 外: 具象を実装
~~x~~

~~{:right}~~
![arch{90%,80%}](onion.png)
~~x~~

~~{:footer}~~
 画像出典: [ドメイン駆動 + オニオンアーキテクチャ概略](https://qiita.com/little_hand_s/items/2040fba15d90b93fc124)
~~x~~