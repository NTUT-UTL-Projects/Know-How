# 如何接手 NTUT-UTL-nRF-Connect-SDK-Monorepo

## 適用對象

1. 要接手 `NTUT-UTL-nRF-Connect-SDK-Monorepo` 的人
2. 想學 nRF Connect SDK 的人
3. 想知道 AD5940/AD5941 如何進行電化學量測的人

## 對象要求

1. 必須熟悉 C 語言
2. 必須會使用 VS code
3. 知曉容器技術 (`Docker` or `Podman`)
4. 稍微看過 `如何接手 EasyEDA 專案`
    - 得知 `ad5941_electrochemical_module_2_layers`, `virus_detector` 的歷史意義
5. 稍微看過 `如何接手 NTUT-UTL-Flutter-Monorepo`
    - 得知 `utl_app` 的歷史意義
    - 得知 `ad5940_temp_debugger` 與 `virus_detector_cart_controller` 缺少的功能

## 開始

### 環境搭建

參考 [GitHub - XIAN-SHENG-576692/nRF-Connect-SDK-Environment](https://github.com/XIAN-SHENG-576692/nRF-Connect-SDK-Environment)
- 若要設定 VS code 使用 podman，請參考 `How to Configure VS Code to Use Podman`

---

### Projects

[GitHub - XIAN-SHENG-576692/utl\_firmware](https://github.com/XIAN-SHENG-576692/utl_firmware)
- v2.9.x
- [GitHub - XIAN-SHENG-576692/ad5940\_applications](https://github.com/XIAN-SHENG-576692/ad5940_applications)

[GitHub - NTUT-UTL-Projects/NTUT-UTL-nRF-Connect-SDK-Monorepo](https://github.com/NTUT-UTL-Projects/NTUT-UTL-nRF-Connect-SDK-Monorepo)
- v3.1.1

```bash
git submodule update --init --recursive
```

nRF Connect for VS Code 基本操作

如何做 CICD

專案缺陷
- GPIO
- `if(buffCount > 1) buffCount = 1;`

TODO
- 解決缺陷
- 嘗試更好的 name convention
- 完成命令控制模塊
- 完成 Mobile App
- 完成現場測試
- 完成 OTA 燒錄功能
