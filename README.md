# xcc-embed-202402-2416060054
嵌入式系统实验仓库

## 仓库说明
本仓库用于《嵌入式系统》课程实验代码管理，所有实验均使用 Keil MDK 开发，目标平台：STM32。
> 仓库规范：禁止网页直接上传文件，全部使用 GitHub Desktop 本地提交，保留完整 commit 记录。

## 实验目录
- 0501_LEDWater：流水灯实验

## 环境依赖
1. Keil MDK-ARM 5
2. 对应芯片固件支持包（DFP）
3. 下载器：ST-Link
4. 代码存放路径：**全英文路径，不含中文、空格**

## 编译与下载步骤
1. 使用 GitHub Desktop 克隆仓库到本地
2. 进入对应实验文件夹，双击 `.uvprojx` 打开 Keil 工程
3. 按下 `F7`（Build）或者 `Rebuild` 编译工程
4. 编译输出：`0 Error(s)` 代表编译成功，生成 hex/axf 文件
5. 连接 ST-Link，`F8` 下载程序到开发板，验证实验现象

## 提交规范
- 修改代码、验证功能后，在 GitHub Desktop 填写提交备注（写明修改内容）
- Commit 后 Push origin 同步到远程仓库
- .gitignore 已配置，自动忽略 Keil 编译产生的中间文件

## 流水灯实验说明（0501_LEDWater）
功能：GPIO 控制LED，实现流水灯循环点亮。
原理：配置GPIO推挽输出，延时函数控制LED轮流翻转电平。
