以下假設Flutter 環境變數 以及flutter sdk 安裝完成
# ```flutter doctor```

## ```flutter doctor``` 環境注意事項

### android studio 安裝完成 並且 安裝cmdline-tool(詳情見android studio 官網)

###  ```輸入flutter doctor --android-licenses``` 並告訴 flutter 接受所有flutter 的協議



配置:
如同android studio 需要將hyper-v 開啟以及 vm-acceration 等環境配置完成。必須先將hyper-v 開啟
# hyper-v 開啟方式
https://learn.microsoft.com/zh-tw/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v

以系統管理員身分開啟 PowerShell 主控台。

執行以下命令：
```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All
```
透過 介面:

以滑鼠右鍵按一下 Windows 鍵，然後選取 \[應用程式與功能\]。

選取相關設定下方右側的 [程式和功能 ]。

選取 [開啟或關閉 Windows 功能]。

選取 [Hyper-V]，然後按一下 [確定]。

# bios Configuration

Restart your computer

On the boot up image, quickly press f12 to enter bios 
(might be a different function key depending on your motherboard)

Go to BIOS configurations (navigation is done with arrow keys enter key to go into or select, and esc to go back)
Go to the M.T.I. tab (should be the default tab)

Go into "Advanced Frequency Settings"

Scroll to "SVM Mode"

You can also look for anything that says virtualization or VT-x if you dont see SVM
Click, enter
Highlight "enable" 

and click enter
Click ESC to go back

Scroll to the right to get to the save tab
Highlight "Save and quit"
Click enter

Your computer will restart. Try to reinstall the SDK Tool, "Android Emulator Hypervisor Driver for AMD Processor (installer) through android studio

