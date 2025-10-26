# 如何接手 NTUT-UTL-Flutter-Monorepo

## 適用對象

以下條件滿足其一者
1. 要接手 `NTUT-UTL-Flutter-Monorepo`
2. 要從零開始開發 Mobile App 的人
3. 想學 Flutter 的人

以下條件皆滿足者
1. 必須有基礎編程技能，且至少懂 OOP
2. 必須知道如何使用 Git，並大概了解 GitHub Actions

## 開始

### 專案位置

- 專案位置
    - https://github.com/NTUT-UTL-Projects/NTUT-UTL-Flutter-Monorepo
- 專案前生_0
    - https://github.com/XIAN-SHENG-576692/utl_app
- 專案前生_1
    - https://github.com/XIAN-SHENG-576692/utl_app_old
    - https://github.com/XIAN-SHENG-576692/flutter_cxs_utils

### 環境搭建

有兩種方法
1. 參考 `如何搭建 Flutter 環境`
2. 參考 [GitHub - XIAN-SHENG-576692/Flutter-Development-Environment-with-VS-Code-using-mingc-android-build-box](https://github.com/XIAN-SHENG-576692/Flutter-Development-Environment-with-VS-Code-using-mingc-android-build-box)
    - 若要設定 VS code 使用 podman，請參考 `How to Configure VS Code to Use Podman`

### 技術細節

架構思路
- [Clean Coder Blog](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html)
- [iT 邦幫忙::關於 Domain-Driven Design 以及他的魅力](https://ithelp.ithome.com.tw/m/articles/10216645)
- [Functional vs Object-Oriented Programming: Key Features](https://www.agiliway.com/functional-and-object-oriented-programming-key-features-and-differences/)

基礎
- 第三方套件管理
    - 如何引用
    - 不聲明引用的後果
        - register 失敗
        - 沒有代碼補全提示

- 專案架構
	- packages
		- bluetooth 技術細節
			- 只能掃描 BLE
			- 使用 `flutter_blue_plus_platform_interface` 額外實現的功能
		- path_provider_utils 的 BUG
	- domains
		- ad5940 與 electrochemical 並非完整，可參考 `專案前生_0`
	- apps
		- `ad5940_temp_debugger` 只是暫時性工具
		- `virus_detector_cart_controller` 缺少解碼 function

- Flutter fundamental
	- commands
	- state management
		- provider
			- context
                - read, select, watch

- 如何設定用戶權限

- 如何更改專案 App 名稱

- `Flutter how to create custom icon`

- GitHub Actions 腳本
