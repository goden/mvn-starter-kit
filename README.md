# mvn-starter-kit
安裝 Maven 前必須安裝 Java，其環境設定可參閱下表：

## 系統需求

| 項目       | 需求                                                         |
| ---------- | ------------------------------------------------------------ |
| JDK        | 以目前Maven最新版本v3.6.3，建議為JDK 1.8                     |
| OS         | 支援Windows, Linux與Mac等主流作業系統                        |
| Hard Drive | Maven 本身安裝最少需約10MB，但Local Maven Repository要視使用情況而定，預期大約接近500MB上下。 |
| Memory     | 沒有明確限制                                                 |

## 下載網址

詳細部份可參考http://maven.apache.org/download.cgi

- Binary tar.gz archive：[apache-maven-3.6.3-bin.tar.gz](https://downloads.apache.org/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.tar.gz) (適用於Linux)
- Binary zip archive：[apache-maven-3.6.3-bin.zip](https://downloads.apache.org/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.zip) (適用於Windows/Mac)

## 設置環境變數

在下載完Maven壓縮檔後，解壓縮至特定目錄(`e.g. C:\maven-3.6.3\或/opt/maven-3.6.3`)

### Windows平台

- **控制台** > **系統及安全性** > **系統** > 左側**系統設定**開啟<u>系統內容</u>視窗
- 點選**環境變數**
- 在**系統變數**列表中，點選**新增**鈕開啟<u>新增系統變數</u>視窗
- 依序在**變數名稱**輸入`MAVEN_HOME`、**變數值**輸入Maven函式庫的絕對路徑(`e.g. C:\maven-3.6.3\或/opt/maven-3.6.3`)
- 輸入完畢後點選**確定**鈕關閉<u>新增系統變數</u>視窗，點選**確定**鈕關閉<u>環境變數</u>視窗。
- 在系統變數列表中選擇`Path`變數，點選**編輯**鈕開啟<u>編輯環境變數</u>視窗，新增`%MAVEN_HOME%\bin`的變數值。
- 新增完畢後依序關閉所有視窗。

