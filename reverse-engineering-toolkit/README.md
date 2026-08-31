# Reverse Engineering Toolkit

这是一个用于授权逆向分析、CTF、沙箱样本和防御性二进制审计的资料包。

## 可用文件

| 文件 | 用途 |
|---|---|
| `SKILL.md` | 平台可加载的技能入口和路由规则 |
| `01-code-obfuscation-deobfuscation.md` | 控制流、字符串、SMC 和常见混淆分析 |
| `02-vm-bytecode-reverse-engineering.md` | 自定义虚拟机、字节码和 opcode 分析 |
| `03-anti-debugging-analysis.md` | Linux/Windows 反调试检测分析 |
| `04-upx-unpacking-analysis.md` | UPX 和常见加壳样本分析 |
| `05-general-reverse-engineering.md` | 通用逆向流程、工具和代码模式 |
| `06-binary-mitigations-ctf.md` | ELF 缓解机制与 CTF 分析 |
| `07-dotnet-reverse-engineering.md` | .NET 反编译、调试和混淆分析 |

## 使用判断

这个目录现在可以被识别为一个技能，因为包含标准入口 `SKILL.md`。编号文档是参考资料，不会自动全部加载；先读取 `SKILL.md`，再按目标选择对应文档。

适用范围：自有程序、明确授权的样本、CTF、隔离沙箱和恶意样本防御分析。分析前保留原始文件并记录哈希，避免直接修改原样本。
