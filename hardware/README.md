# 基板と電子部品
PLEN2-Projectは公式が販売終了しているので基板を購入できません。  
自作で基板の作製が必要です。KiCAD+PCBwayでPCBを作製する方法はありますが  
私はディスクリートでトライします。  
## 構成検討
不要な物を削り本家に比べてシュリンク可能。
システム構成はマイコン(ESP32)とマルチプレクサ(4051)またはPCA9685、サーボモーター×6個（下半身のみ）、LED×2個にシュリンク可能。smallスタート。  
PLEN2(本家)はジャイロ(MPU-6050)がついているがフィードバック制御をしていないので意味がない。不要。
BLEはESP32にBluetoothモジュールが内臓されているため不要。  
本家アプリがあればできたこともEOLでアプリストアから削除されているため不要。

## 頭部基板
LEDx2、BLE(Bluetooth)、IMU5060(ジャイロ)、MAX3486(RS-485通信)からLEDx2のみへ変更。
### LED spec
Vf：3.5V Green

## 基板構成
<img width="1293" height="497" alt="image" src="https://github.com/user-attachments/assets/2cdacd9e-8b7c-451f-893d-f5e740013b1e" />
## 回路図  
(https://github.com/user-attachments/files/31713528/PLEN2.pdf)

## マルチプレクサ 3個
<img width="750" height="500" alt="image" src="https://github.com/user-attachments/assets/98b432e5-3d72-4072-a9fb-7d61e9f9a3e6" />



# リファレンス
## 頭部基板
https://github.com/plenprojectcompany/plen-HeadBoard
## 胸部基板
https://github.com/plenprojectcompany/plen-ControlBoard?utm_source=chatgpt.com
## SCL Viewer
https://www.altium.com/viewer/?utm_source=chatgpt.com  
## 従来基板  回路図
<img width="1127" height="1632" alt="image" src="https://github.com/user-attachments/assets/d28f6316-4178-41bc-9b06-effb7290ab7b" />
<img width="1125" height="1632" alt="image" src="https://github.com/user-attachments/assets/a0e2abba-4033-4238-aa57-f0bd298f54bb" />


