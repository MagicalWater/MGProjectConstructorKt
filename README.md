# MGProjectConstructorKt
[ ![Download](https://api.bintray.com/packages/water/mgbase/mg-project-constructor-kt/images/download.svg) ](https://bintray.com/water/mgbase/mg-project-constructor-kt/_latestVersion) 
![](https://img.shields.io/badge/language-kotlin-orange.svg)  

一個Android APP專案的基底  

包含以下功能的封裝:  
1. 動畫位移相關layout  
2. api request 單獨拉出, 供自訂widget, 不屬於 aty 與 fgt 的地方使用  
3. fragment跳轉 單獨拉出, 供fragment內部有子freagment跳轉使用  
4. activity 跟 fragment 的基底已經封裝好了 api request 跟 fragment跳轉  
5. qrcode 掃描view的封裝(MGZbarView: 接入bga-qrcode-zbar)  
6. 圖片選擇器調用封裝(MGPhotoPickerHelper)  
7. 多國語系(MGLocalManager)  

## 版本  
0.2.0 - 修改 MGUrlRequest 抓取檔案的方式(可抓取字串反序列化/下載檔案), 修正 無法上傳檔案  
0.1.9 - 頁面跳轉呼叫的 fgtShow(param) 加入可帶入Any, 在內部判斷類型調用  
0.1.8 - 修改 MGFgtManager 呼叫回退時的出場動畫,　由靜止不動改為透明淡出  
0.1.7 - 修正因依賴 mg-utils-kt 的庫 更新後造成的圖片讀取失敗  
0.1.6 - 修復app縮小太久導致頁面被銷毀重新進入 activity 的 onCreate 方法時, 重新設置fragmentManager造成的頁面初始化資訊錯誤  

## 添加依賴  

### Gradle  
compile 'org.mgwater.mgbase:mg-project-constructor-kt:{version}'  
( 其中 {version} 請自行替入此版號 [ ![Download](https://api.bintray.com/packages/water/mgbase/mg-project-constructor-kt/images/download.svg) ](https://bintray.com/water/mgbase/mg-project-constructor-kt/_latestVersion) )
