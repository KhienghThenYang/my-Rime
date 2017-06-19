## 顯示輸入法候選欄

不熟悉如何定製的同學請先閱讀 [**〔定製指南〕**](https://github.com/rime/home/wiki/CustomizationGuide) 。

同文輸入法主題與配色方案的設定檔命名格式爲 `*.trime.yaml` ，用戶對其定製的自定義檔命名格式爲 `*.trime.custom.yaml` 。

軟件默認應用的主題與配色方案爲 `trime.yaml` ，本文以此爲例，編寫與其對應的自定義檔 `trime.custom.yaml` ，向自定義檔中添加如下代碼並保存。

```
# trime.custom.yaml
# encoding: utf-8

patch:
  "style/layout/max_entries": 5 # 此處爲候選項的個數，過多會導致候選項顯示不完整，參考範圍 3-5
  "style/layout/min_length": 1 # 此處不要修改，以確保可以顯示候選項
  "style/layout/sticky_lines": 0 # 此處爲候選項固頂數，過多同樣會導致候選項顯示不完整，參考範圍 0-1
```

或者 [**此處右鍵另存爲**](https://raw.githubusercontent.com/ThomasHawaiiKing/my-Rime/master/forced_candidate/trime.custom.yaml) 可下載示範設定檔。

將 `trime.custom.yaml` 放入 Android 設備的 `rime/` 目錄，打開同文輸入法主界面，點擊部署等待完成即可。此時輸入法即可顯示出候選項。

一般按鍵 `，` 和 `。` 爲候選項的翻頁鍵（僅當存在候選項時可用），若仍無法翻頁，可參閱 [**〔trime.yaml詳解#佈局调整〕**](https://github.com/osfans/trime/wiki/trime.yaml%E8%A9%B3%E8%A7%A3#%E4%BD%88%E5%B1%80%E8%B0%83%E6%95%B4) 指定鍵盤中的一對按鍵爲翻頁鍵。

## <br />

“叫我 **慶天** ！” “好的，小七！”
