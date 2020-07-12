# InariBako
VRChat Prefab Collection for SDK2.

## Requirements
* VRChat SDK2
* VRC StarterKit
  * https://booth.pm/ja/items/979837
  * https://gitlab.com/vrchat_projects_momoma/vrc_starterkit

See also README in each assets.

## Components
* `Events`
  * `ActivateTrigger.cs` を使ったイベントハンドリングシステム。
  * Event handling system based on `ActivateTrigger.cs`.
* `Mods/`
  * 他のアセットの拡張。
  * Extensions for other assets.
* `SafeSpawner`
  * 大量の物理演算つきピックアップを動かすためのSpawn。オーナーのみが操作でき、シミュレーションもオーナーだけで行う。
  * Spawn many pickups with physics. Which simulated controllable only on owner.
* `Sync`
  * `SendRPC` を利用した `OwnerLocal` と `MasterLocal` の実装。
  * `OwnerLocal` and `MasterLocal` trigger with `SendRPC`.

## License
MIT License. Ses [LICENSE](LICENSE).
