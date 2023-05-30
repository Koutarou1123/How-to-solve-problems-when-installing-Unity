# How-to-solve-problems-when-installing-unity

## 概要
---
このリポジトリは私がUnityインストール時に公式通りに行い詰まった箇所の解決方法を記す．
 
1.https://docs.unity3d.com/hub/manual/InstallHub.html#install-hub-linux

mistake command
```
sudo sh -c 'echo "deb [signedby=/usr/share/keyrings/Unity_Technologies_ApS.gpg] https://hub.unity3d.com/linux/repos/deb stable main" > /etc/apt/sources.list.d/unityhub.list'
```
上記のコマンドだと，NO_PUBKEYと言われてしまう．
<br>
<br>

correct command
```
sudo sh -c 'echo "deb [signed-by=/usr/share/keyrings/Unity_Technologies_ApS.gpg] https://hub.unity3d.com/linux/repos/deb stable main" > /etc/apt/sources.list.d/unityhub.list'
```


# REFERENCE
