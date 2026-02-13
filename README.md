# easinote-mcp-guide
本文主要讲述关于希沃白板的 MCP 功能。

有关技术细节，请自行[反编译](https://www.jetbrains.com.cn/decompiler/download/download-thanks.html?platform=windows64)`【希沃白板安装目录】\EasiNote5_5.2.4.xxxx\Main\EasiNote.McpServer.dll`。

<!-- 点击以上链接下载 dotPeek -->

~~希沃官方 Agent：敬请期待超能小希。~~

## 启用方法
1. 创建文件夹：`%APPDATA%\Seewo\SeewoAIVoiceAssistant\McpServers`。

此时系统会创建一个配置文件（见下）。

2. 查看文件`%APPDATA%\Seewo\SeewoAIVoiceAssistant\McpServers\EasiNote.mcp.json`。

它应该长这样：
```jsonc
{
  "names": [
    "EasiNote"
  ],
  "description": "\u5E0C\u6C83\u767D\u677F 5",
  "servers": [
    {
      "type": "http",
      "pid": 114514, // 这里可能不同，但不重要
      "processName": "EasiNote.exe",
      "url": "http://127.0.0.1:11451/mcp" // 记下这一行，很重要！端口号是随机的
    }
  ]
}
```
3. 将此链接复制到你的 AI 客户端。

配置如下：（以 [Qwen Desktop](https://qwen.ai/download) 为例）

![Config](https://github.com/user-attachments/assets/da9a6ae1-5599-4d30-a2c2-db82637f5bf5)

## 已知问题
根本连不上。

![Error](https://github.com/user-attachments/assets/55bc11a7-b702-4404-b675-0adee617b935)
<!--
<img width="2815" height="1687" alt="image" src="https://github.com/user-attachments/assets/eba20529-447c-4756-ad19-8de03bcc90b8" />
-->
