# InariBako
VRChat Prefab Collection for SDK2.

Documentation is !!WIP!!

## Requirements
* VRChat SDK2
* VRC StarterKit
  * https://booth.pm/ja/items/979837
  * https://gitlab.com/vrchat_projects_momoma/vrc_starterkit

## Components
* `Events`
  * `ActivateTrigger.cs` を使ったイベントハンドリングシステム。
  * Event handling system based on `ActivateTrigger.cs`.
* `Mods/`
  * 他のアセットの拡張。
  * Extensions for other assets.
* `SafeSpawner`
  * 大量の物理演算つきピックアップを動かすためのSpawn。オーナーのみが操作でき、シミュレーションもオーナーだけで行う。
  * `SafeSpawner` のカスタムアクション `Spawn` でスポーン、 `DespawnAllOwned` で自身の所有するアイテムを消し、 `DespawnAll` でワールド中の全てのアイテムを消す。
  * コライダーを変更する場合は `SpawnedItem` に加えて `NoOwner` も変更すること。
  * 地面のみと接触する `Layer` を作成し、 `NoOwner` に設定するとより安定します。
  * Spawn many pickups with physics. Which simulated controllable only on owner.
* `Sync`
  * `SendRPC` を利用した `OwnerLocal` と `MasterLocal` の実装。カスタムアクション `Trigger` を実行すると、`Owner` または `Master` でのみ `Action` が実行される。
  * `OwnerLocal` and `MasterLocal` trigger with `SendRPC`.

## License
MIT License. Ses [LICENSE](LICENSE).
