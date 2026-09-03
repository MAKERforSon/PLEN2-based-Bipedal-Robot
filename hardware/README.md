# 基板と電子部品
PLEN2-Projectは公式が販売終了しているので基板を購入できません。  
自作で基板の作製が必要です。KiCAD+PCBwayでPCBを作製する方法はありますが  
私はディスクリートでトライします。  
## 構成検討の結果
本家に比べてかなりシュリンクできる。
システム構成はマイコン(ESP32)とマルチプレクサ(4051)またはPCA9685、サーボモーター×6個（下半身のみ）、LED×2個にシュリンク可能。最小構成でsmallスタート。  
PLEN2(本家)はジャイロ(MPU-6050)がついているがフィードバック制御をしていないので用途がない。なくて問題ない。  
BLEはESP32にBluetoothモジュールが内臓されているため不要。  
本家アプリが現役でいればできたこともEOLでアプリストアから削除されているため不要。

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


