# Fuwat Mouse AZ1U

https://github.com/user-attachments/assets/fa95952d-c69b-4201-aef6-798942abb8b3

## Project Summary

This project is a compact, handheld wireless trackball device ("air mouse") built using the ultra-small AZ1UBALL trackball and Seeed Studio's Xiao BLE (nRF52840) microcontroller. The device is designed for one-handed operation, with a body measuring just 70 mm in length and 22 mm in width—small enough to fit comfortably in the palm of your hand.

- **One-handed operation:** Enables left/right mouse clicks, cursor movement, scrolling, D-pad actions, and volume control.
- **10 physical buttons:** Allows diverse input and control.
- **Multi-layer support via ZMK firmware:** Switch between mouse control, shortcuts, and device selection, all on one device.
- **Live customization:** Modify keymaps and layers in real-time using ZMK Studio.
- **Highly compact:** All features packed into a tiny enclosure.

このプロジェクトは、超小型トラックボール AZ1UBALL と Seeed Studio 製 Xiao BLE (nRF52840) マイコンを用いて、片手で操作可能な小型ワイヤレス・トラックボールデバイス（「エアマウス」）です。デバイス本体は長さわずか 70mm、幅 22mm と非常に小型で、手のひらに収まるサイズ感を実現しています。
- 片手操作: 左右クリック、カーソル移動、スクロール、方向キー操作、音量調整が可能。
- 10個の物理ボタン: 多様な入力やコントロールを実現。
- ZMK ファームウェアによるマルチレイヤー対応: マウス操作、ショートカット、デバイス切り替えを1台で行える。
- リアルタイムカスタマイズ: ZMK Studio を使用してキーマップやレイヤーを即時に変更可能。
- 高いコンパクト性: すべての機能を小型筐体に集約。

販売は未定です。
  
## Article
- https://note.com/amgskobo/n/n39ae0e2d3ca7
- https://note.com/amgskobo/n/naa46139e9779
## Requirements

- [firmware (TBA) ](https://github.com/amgskobo/config-fuwat-mouse)
- 1x Xiao BLE (nRF52840)
- 10x micro key swtich
- 10x 1N4148 diode
- 500mAh Lipo battery

## Key Mapping

### Layer 0 [MOUSE]
<img width="666" height="590" alt="" src="https://github.com/user-attachments/assets/5468c2e0-df32-4cac-80b6-d73b0897d059" />

* &layer_mkp_hold_tap
  * Hold / ホールド ==> Layer activate / レイヤー有効化
  * Tap / タップ　==> Click　/ クリック動作
* &mkp_hold_tap
  * Hold / ホールド ==> MOUSE KEY3 (MIDDLE CLICK) / ミドルクリック
  * Tap / タップ　==> MOUSE KEY2 (RIGHT CLICK) /　右クリック

### Layer 1 [SCROLL]
<img width="394"  alt="" src="https://github.com/user-attachments/assets/80dea7a4-11ca-4780-aeb1-2178cb37e201" />

### Layer 2 [MEDIA]
<img width="394"  alt="" src="https://github.com/user-attachments/assets/ccdbb93c-034e-47a1-af9d-3916df1b4b27" />

### Layer 3 [DEV] 
Enable with press 2 keys by this order. 
  1. hold layer2 key　/ Layer2 をホールドした後
  2. hold layer1 key　/ Layer1 をホールド
<img width="394" height="553" alt="" src="https://github.com/user-attachments/assets/66d3a5aa-e41d-4418-a01b-260a979bf216" />

* &dev -- Development key / tap_dance / Clicks 
1. &hw_soft_off / SoftOff (hold 2 seconds) / 2秒長押しでソフトオフ
2. &sys_reset / System Reset /　システムをリセット
3. &bootloader / Bootloader /　ブートローダーを起動
4. &bt BT_CLR / CLear pairing /　接続中のペアリングをリセット
5. &bt BT_CLR_ALL> / Clear all pairing /　全てのペアリングをリセット
## Author

- https://x.com/amgskobo

---

*For questions and support, please open an issue on GitHub or X.
質問やサポートについては、GitHubで issue または Xにて*
