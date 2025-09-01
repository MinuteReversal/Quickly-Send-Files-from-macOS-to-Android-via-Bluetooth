# Quickly Send Files from macOS to Android via Bluetooth

## Overview
Add a custom Automator Quick Action to Finder’s right-click menu, allowing you to send selected files to an Android phone using Bluetooth File Exchange.

## Steps

1. Open **Automator** and create a new “Quick Action”.
2. Set “Workflow receives current” to “files or folders”.
3. In the left sidebar, type “shell” in the search box to quickly find the **Run Shell Script** action.
4. Drag **Run Shell Script** into the workflow area.
5. Set “Pass input” (above the script area) to “as arguments”.
6. Enter the following script:

    ```bash
    open -a "Bluetooth File Exchange" "$@"
    ```

7. Save and name the workflow (e.g., “Send via Bluetooth”).
8. In Finder, right-click any file and choose “Quick Actions” → “Send via Bluetooth”.
9. Make sure your Android phone’s Bluetooth is enabled and ready to receive files. Follow the prompts to complete the transfer.

## Notes

- The “Run Shell Script” action can be found by searching for “shell” in Automator’s sidebar.
- Your Android device must be discoverable and able to receive files via Bluetooth.
- This method uses macOS’s built-in Bluetooth File Exchange.



# macOS 快速通过蓝牙发送文件到安卓手机

## 功能简介
在 Finder 右键选中文件，通过自定义 Automator 快速操作，直接用“蓝牙文件交换”发送文件到安卓手机。

## 操作步骤

1. 打开 **Automator**，新建“快速操作”。
2. 设置“工作流程接收当前”类型为“文件或文件夹”。
3. 在左侧导航栏的搜索框输入“shell”，快速找到 **运行 Shell 脚本** 操作。
4. 将 **运行 Shell 脚本** 拖到右侧工作区。
5. 将“传递输入”设置为“作为自变量”。
6. 输入以下脚本内容：

    ```bash
    open -a "Bluetooth File Exchange" "$@"
    ```

7. 保存并命名（如“用蓝牙发送”）。
8. 在 Finder 里右键文件，选择“快速操作”→“用蓝牙发送”。
9. 手机蓝牙需处于可接收状态，按提示完成文件接收。

## 注意事项

- “运行 Shell 脚本”操作可通过搜索“shell”快速找到。
- 安卓手机需打开蓝牙并允许接收文件。
- 该方法适用于 macOS 原生“蓝牙文件交换”应用。

<img width="545" height="599" alt="截屏2025-09-01 10 32 56" src="https://github.com/user-attachments/assets/e07f4fb1-f89f-4ec6-8922-97937f906097" />
<img width="710" height="464" alt="截屏2025-09-01 10 26 52" src="https://github.com/user-attachments/assets/e9c2a11f-a0c2-47c9-a58b-7c87c6302c97" />
