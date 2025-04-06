# Refined Storage → Applied Energistics 2 移行ガイド

## RS: 最小構成
Refined Storageでアイテムの出し入れができる倉庫を作成するためには、以下のアイテムが必要です:


<details><summary>コントローラー</summary>

エネルギーを受け取り、接続された機械を管理します。ネットワーク内に1つだけ設置する必要があります。

![Controller](recipes/refinedstorage/controller.png)</details>


<details><summary>グリッド</summary>

ネットワーク内のアイテムの出し入れができます。

![Grid](recipes/refinedstorage/grid.png)</details>


<details><summary>ストレージブロック</summary>

1千ストレージブロックでは、任意のアイテムを1000個まで保管できます。
空のストレージブロックを`Shift`+`右クリック`して、ストレージパーツを取り外せます。

![1k Storage Block](recipes/refinedstorage/1k_storage_block.png)</details>


また、コントローラーへエネルギーを供給する必要がありますが、Refined Storageに発電機はありません。
MekanismやPowah!などの発電機を使用してください。

![Minimal Configuration](refinedstorage/minimal.png)

スペースを節約したい場合は、次のアイテムで代用できます:

<details><summary>携帯グリッド</summary>

持ち運び・設置共に可能なグリッドです。ストレージディスクを挿入する必要があります。

![Portable Grid](recipes/refinedstorage/portable_grid.png)</details>



## AE2: 最小構成
Applied Energistics 2で同様の構成を作成するには、以下のアイテムが必要です:


<details><summary>MEチェスト</summary>

側面からストレージセルを挿入すると、上面のターミナル部からアイテムを出し入れできます。

![ME Chest](recipes/ae2/network_blocks_storage_chest.png)</details>


<details><summary>MEアイテムストレージセル</summary>

1k MEアイテムストレージセルでは、4160個-8128個のアイテムを、最大63種保管できます。

![1k ME Item Storage Cell](recipes/ae2/network_cells_item_storage_cell_1k.png)</details>

<details><summary>Crystal Resonance Generator (任意)</summary>

設置すると20AE/t=40RF/tのエネルギーを供給します。エネルギーが不足する場合は、火力発電機を使用するか、他MODの発電機を接続してください。

![Crystal Resonance Generator](recipes/ae2/network_crystal_resonance_generator.png)</details>

![Minimal Configuration](ae2/minimal.png)



## RS: 複数のディスクを管理する

ストレージブロックを以下のアイテムで置き換えてください:


<details><summary>ストレージディスク</summary>

ストレージブロックと同様に、アイテムを保管できます。ディスクドライブに挿入することで機能します。

![Storage Disk](recipes/refinedstorage/1k_storage_disk.png)</details>

<details><summary>ディスクドライブ</summary>

ストレージディスクを最大8枚挿入できます。

![Disk Drive](recipes/refinedstorage/disk_drive.png)</details>

![Multiple Disks](refinedstorage/multiple-disks.png)



## AE2: 複数のセルを管理する

MEチェストを以下のアイテムで置き換えてください:

<details><summary>MEドライブ</summary>

MEアイテムストレージセルを最大10枚挿入できます。

![MEドライブ](recipes/ae2/network_blocks_storage_drive.png)</details>

<details><summary>フルーシュのMEガラスケーブル</summary>

MEネットワークにおけるケーブルの役割を果たします。

![Fluix ME Glass Cable](recipes/ae2/network_cables_glass_fluix.png)</details>

<details><summary>MEターミナル</summary>

MEネットワーク内のアイテムの出し入れができます。

![ME Terminal](recipes/ae2/network_parts_terminals.png)</details>

![Multiple Cells](ae2/multiple-cells.png)

他MODの発電機を使用する場合は、追加で以下のアイテムが必要です:

<details><summary>エナジーアクセプター</summary>

受け取ったエネルギーを変換し、ネットワークへ供給します。

![Energy Acceptor](recipes/ae2/network_blocks_energy_energy_acceptor.png)</details>



## RS: 手動クラフト

ネットワーク上のアイテムを用いて作業台クラフトを行うには、グリッドを以下のアイテムで置き換えてください:

<details><summary>クラフトグリッド</summary>

作業台機能が内蔵されたグリッドです。JEI/REI/EMIから直接レシピを配置できます。

![Crafting Grid](recipes/refinedstorage/crafting_grid_crafting_grid.png)</details>



## AE2: 手動クラフト

ネットワーク上のアイテムを用いて作業台クラフトを行うには、MEターミナルを以下のアイテムで置き換えてください:

<details><summary>MEクラフトターミナル</summary>

作業台機能が内蔵されたMEターミナルです。RS同様に、JEI/REI/EMIから直接レシピを配置できます。

![ME Crafting Terminal](recipes/ae2/network_parts_terminals_crafting.png)</details>



## RS: 自動作業台クラフト

Refined Storageで作業台クラフトを自動化するには、以下のアイテムが必要です:

<details><summary>パターン</summary>

レシピを保管します。

![Pattern](recipes/refinedstorage/pattern.png)</details>

<details><summary>パターングリッド</summary>

レシピをパターンへ書き込みます。レシピビューアから直接書き込むこともできます。

精密モードがオフの場合、NBTは無視され、タグが共通の他アイテムを使用してクラフトを行うようになります。例えば、チェストの作成にどんな種類の木材でも使用できるようになります。

![Pattern Grid](recipes/refinedstorage/pattern_grid_pattern_grid.png)</details>

<details><summary>クラフター</summary>

登録されたパターン通りにアイテムをクラフトします。最大9個のパターンを挿入できます。

![Crafter](recipes/refinedstorage/crafter.png)</details>

![Crafter](refinedstorage/crafter.png)

任意のグリッド上で`クラフト`と表記されたアイテムをクリックすることで、クラフトの発注を行えます。
既にネットワーク上に存在するアイテムを追加発注するには、アイテムを`Ctrl`+`Shift`+`クリック`してください。



## AE2: 自動作業台クラフト

AE2で作業台クラフトを自動化するには、以下のアイテムが必要です:

<details><summary>ブランクパターン</summary>

レシピを保管します。

![Blank Pattern](recipes/ae2/network_crafting_patterns_blank.png)</details>

<details><summary>MEパターンエンコーディングターミナル</summary>

レシピをパターンへ書き込みます。同様に、レシピビューアから直接書き込むこともできます。

`置換有効`状態は、RSの精密モードに相当します。

![ME Pattern Encoding Terminal](recipes/ae2/network_parts_terminals_pattern_encoding.png)</details>

<details><summary>分子組立機</summary>

登録されたパターンに応じてアイテムを受け取り、クラフトを行います。パターンを1個だけ挿入できます。

![Molecular Assembler](recipes/ae2/network_crafting_molecular_assembler.png)</details>

<details><summary>MEパターンプロバイダー</summary>

登録されたパターンに応じて、周囲の機械へアイテムを供給します。最大9個のパターンを挿入できます。

空の分子組立機に隣接させた場合、分子組立機を使用してクラフトを行い、成果物を自動で取り込みます。

![ME Pattern Provider](recipes/ae2/network_blocks_pattern_providers_interface.png)</details>

<details><summary>クラフティングストレージ</summary>

ネットワークの自動クラフトを担当するマルチブロック設備、**クラフトCPU**の構築に使用します。

![Crafting Storage](recipes/ae2/network_crafting_1k_cpu_crafting_storage.png)

</details>

![Molecular Assembler](ae2/molecular-assembler.png)

任意のMEターミナル上で`クラフト`と表記されたアイテムをクリックすることで、クラフトの発注を行えます。既にネットワーク上に存在するアイテムを追加発注するには、アイテムを`ミドルクリック`してください。

大きなストレージを持つクラフトCPUは、自動クラフトでたくさんのアイテムを取り扱うことができますが、1つのCPUが複数の自動クラフトを実行することはできません。複数の自動クラフトを発注するには、CPUを複数台用意してください。
