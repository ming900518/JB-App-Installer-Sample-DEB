# JB-App-Installer-Sample-DEB

A sample DEB file using AppSync, appinst and signer.sh to fake sign and install apps on Jailbroken iDevices.

這是一個範例DEB檔案，使用AppSync、appinst和signer.sh進行fake sign後，安裝App至已越獄的iDevice上。

### Disclaimer: This sample should not be modified to distribute pirated iOS Apps, I'm not responsible to any legal responsibility made by any DEB package based on this sample.

### 免責聲明：本範例不應該被修改用來散播盜版iOS App，任何基於本範例的DEB檔如有衍生任何法律責任，本人概不負責。

## How to
The following steps uses macOS as an example, please install DPKG with brew first.

Step 1. Download and unzip the source code

Step 2. Rename the App's IPA file to ```Unsigned.ipa```, replacing the file in```com.orgname.packagename/var/mobile```

Step 3. Modify the ```control``` file in```com.orgname.packagename/DEBIAN```, all the strings enclosed by \[] needs to be replaced

Step 4. Rename the ```com.orgname.packagename```

Step 5. Open the terminal and cd to ```JB-App-Installer-Sample-DEB```

Step 6. Enter the command to package ```dpkg -b [the directory name modified in Step 4]```

## 如何使用
以下以macOS為例，請先使用brew安裝DPKG

Step 1. 下載原始碼並解壓縮

Step 2. 將App的IPA檔改名為```Unsigned.ipa```，取代```com.orgname.packagename/var/mobile```中的檔案

Step 3. 修改```com.orgname.packagename/DEBIAN```中的```control```檔案，所有以 \[ ] 匡起來的字串都需要被替換掉

Step 4. 將```com.orgname.packagename```目錄改名

Step 5. 開啟終端機，cd至```JB-App-Installer-Sample-DEB```

Step 6. 輸入指令進行打包```dpkg -b [Step 4所設定的目錄名稱]```

### Before installing the DEB file modified by this sample, you should add https://cydia.akemi.ai/ repo to your package manager first.
### 安裝修改自本範例的DEB前，請先在套件管理工具中加入 https://cydia.akemi.ai/ 軟體源
