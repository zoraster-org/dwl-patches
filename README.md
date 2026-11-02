# dwl-patches

Patches applied on top of nixpkgs' [dwl](https://codeberg.org/dwl/dwl) by
[install-script](https://github.com/zoraster-org/install-script), which
consumes this repo as the `dwl-patches-src` flake input and applies every
`*.patch` here in the order listed in its dwl override.

| Patch | What it does |
|---|---|
| `dwl-gaps.patch` | gaps between tiled windows |
| `dwl-ipc-v2.patch` | the community `ipc` patch (dwl-ipc-unstable-v2 protocol, for waybar's dwl module); by choc, from the dwl patches collection |
| `dwl-rule-geom.patch` | optional initial geometry (position and size) on window rules |
| `dwl-software-cursors.patch` | software cursor compositing when `DWL_SOFTWARE_CURSORS` is set, for hypervisors whose hardware cursor plane doesn't render (Parallels virtio-gpu) |

Patches to dwl are derived from dwl and carry its licence, GPL-3.0 (see `LICENSE`).
