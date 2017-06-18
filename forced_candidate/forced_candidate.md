# 顯示輸入法候選欄

不熟悉如何定製的同學請先閱讀 [**〔定製指南〕**](https://github.com/rime/home/wiki/CustomizationGuide) 。

本設定檔是同文輸入法主題的自定義檔。

同文輸入法主題與配色方案的設定檔命名格式爲 `*.trime.yaml` ，用戶對其定製的自定義檔命名格式爲 `*.trime.custom.yaml` 。

軟件默認應用的主題與配色方案爲 `trime.yaml` ，此處以此爲例，編寫對應的自定義檔 `trime.custom.yaml` ，添加如下代碼，使其可以顯示出候選項。

```
# trime.custom.yaml
# encoding: utf-8

patch:
  "style/layout/max_entries": 5 # 此處爲候選項的個數，個數過多會導致候選項顯示不完整
  "style/layout/min_length": 1 # 此處不要修改，以確保可以顯示候選項

```

將 `trime.custom.yaml` 放入手機的 `rime/` 目錄，打開同文輸入法主界面點擊部署即可。

一般 `，` 和 `。` 爲候選項的翻頁鍵（僅當存在候選項時可用）,若仍無法翻頁，可參閱 [**〔trime.yaml詳解#佈局调整〕**](https://github.com/osfans/trime/wiki/trime.yaml%E8%A9%B3%E8%A7%A3#%E4%BD%88%E5%B1%80%E8%B0%83%E6%95%B4) 指定鍵盤中的一對按鍵爲翻頁鍵。

“叫我 **慶天** ！” “好的，小七！”