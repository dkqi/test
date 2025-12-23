## 1.TortoiseGit 下载地址

```
https://tortoisegit.org/download/
```

![alt text](<../images/TortoiseGit 下载.png>)

## 2. TortoiseGit 汉化地址

```
https://download.tortoisegit.org/tgit/2.18.0.0/TortoiseGit-LanguagePack-2.18.0.0-64bit-zh_CN.msi
```

![alt text](<../images/TortoiseGit 汉化.png>)

## 3. TortoiseGit 图标覆盖设置

```
参考：https://www.cnblogs.com/daihaoliulingyi601/p/18927386
```

### 步骤 1：进入任意文件夹，右键

![alt text](../images/TortoiseGit-1进入设置.png)

### 步骤 2：勾选图标覆盖

![alt text](../images/TortoiseGit-2勾选图标覆盖.png)

### 步骤 3：启动注册表编辑器

![alt text](../images/TortoiseGit-3启动注册表编辑器.png)

### 步骤 4：打开注册表后，会自动跳转到:HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\ShellIconOverlayIdentifiers 这一项;把每一项'Tortoise 开头的文件'排序到最前面

![alt text](../images/TortoiseGit-4注册表文件排序.png)

### 步骤 5：打开"任务管理器"（按 Esc+Shift+Ctrl），选择 'Windows 资源管理器' 右键,重启服务

![alt text](../images/TortoiseGit-5重启任务管理器.png)
