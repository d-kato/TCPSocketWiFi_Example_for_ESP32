# TCPSocketWiFi_Example_for_ESP32
GR-LYCHEE上のESP32をATコマンドで操作するサンプルプログラムです。  
GR-LYCHEEの開発環境については、[GR-LYCHEE用オフライン開発環境の手順](https://developer.mbed.org/users/dkato/notebook/offline-development-lychee-langja/)を参照ください。

ビルドする前に``mbed_app.json``の SSID と Passwordを変更してください。  
```json
{
    "config": {
        "wifi-ssid": {
            "help": "WiFi SSID",
            "value": "\"SSID\""
        },
        "wifi-password": {
            "help": "WiFi Password",
            "value": "\"Password\""
        }
    }
}
```

## ESP32をATコマンド用のファームウェアに書き換える
本サンプルプログラムを使用する際は``ESP32をATコマンド用のファームウェア「esp32-at」``に書き換える必要があります。  
(GR-LYCHEEのESP32には初期ファームとして「esp32-at」が書き込まれているため、そのままご利用になれます。)  
書き換え方法については下記を参照ください。  
https://github.com/d-kato/GR-LYCHEE_ESP32_Serial_Bridge  
