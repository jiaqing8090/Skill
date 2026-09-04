# Minis Skills 技能库

> 从 Codex eni-solo v4.0.0 包里提取的可复用技能知识库，按小羊助手（Minis）技能规范整理。
> 每个技能目录含 `SKILL.md`（YAML frontmatter 定义 `name`/`description`），**直接可导入使用**。

## 目录
- [导入方式](#导入方式)
- [技能清单](#技能清单)
  - [A. 逆向工程（核心）](#a-逆向工程核心)
  - [B. 游戏安全 / 逆向](#b-游戏安全--逆向)
  - [C. 渗透测试 / 红队](#c-渗透测试--红队)
  - [D. Web 漏洞细节包（redteam）](#d-web-漏洞细节包redteam)
  - [E. API / 浏览器 / 自动化](#e-api--浏览器--自动化)
  - [F. 方法论 / 流程 / 平台](#f-方法论--流程--平台)
- [使用边界](#使用边界)

---

## 导入方式

1. 把小羊助手 skills 目录指向本仓库，或下载仓库后解压。
2. 将需要的技能目录放进 Minis skills 目录。
3. 小羊助手通过每个技能目录的 `SKILL.md` 前部的 YAML frontmatter 识别技能名与触发描述。

---

## 技能清单

> 一行一技能：`技能名` — 一句话功能（触发场景）

### A. 逆向工程（核心）

| 技能 | 功能 |
|---|---|
| `asm-analysis` | 深度汇编逆向分析 — GDB/LLDB/r2/Frida/angr/strace 全链路协同 |
| `eni-apk-reverse` | Android APK 逆向 — 解包、jadx 反编译、smali 修改、重打包、Frida Hook |
| `eni-js-reverse` | 前端 JS 逆向 — 签名、加密参数还原、a_bogus/X-Bogus |
| `eni-ida-reverse` / `ida-reverse` | IDA 逆向工作流 |
| `eni-radare2` | radare2 逆向分析 |
| `eni-mobile-reverse` | 移动端（App）逆向 |
| `eni-binary-diff` | 二进制差异对比 (±diff) |
| `eni-reverse-deep` | 深度逆向技法 |
| `eni-reverse-ref` | 逆向参考手册（459KB 资料）|
| `eni-reverse-workflow` | 逆向通用流程编排 |
| `eni-unpack-reverse-lab` | 脱壳 / 加壳还原实验室 |
| `linker-fake-load-unwrapper` | Android ELF linker 伪 LOAD 加固脱壳通杀 |
| `elf-local-auth-patcher` | 自有/授权 ELF 本地授权补丁（AArch64 分支 patch） |
| `eni-blackbox-reverse-boost` | 黑盒逆向 + 本地 Windows 二进制安全审计 |
| `eni-pwn-chain` | 漏洞利用链（pwn） |
| `eni-malware-analysis` | 恶意样本分析 |
| `eni-memory-forensics` | 内存取证分析 |
| `xigong-funk-hikari` | 西宫 Funk Hikari 逆向工具集 |
| `yingan-tuoxiu` / `西宫影安老版本脱修` | 西宫影安脱壳修复（老版本） |
| `eni-reverselab-platform` | 完整逆向实验室 — 197 篇知识库 + MCP 工具 + 多板路由（最大体量 6.1MB） |
| `eni-reverselab-bridge` | 逆向实验室桥接 |
| `eni-core` | 核心路由/执行引擎 |

### B. 游戏安全 / 逆向

| 技能 | 功能 |
|---|---|
| `eni-game-hacking` | 游戏逆向/辅助开发 |
| `eni-game-security` | 游戏安全研究 |
| `eni-game-cheat-lab-workflow` | 游戏外挂/修改器实验室工作流 |
| `eni-cf-security-lab-router` | FPS(CF/穿越火线) 安全实验室路由器 |
| `zzy-codex5.6` | 游戏安全 & 逆向技能集合包 |
| `外挂逆向skills` | 游戏外挂逆向 & 通用逆向集合 |
| `shiyi-pentest-gate` | 渗透测试授权归一化执行器 |
| `game-assets` | 游戏美术资产生成（像素/HD 精灵、纹理、地图）——非安全 |

### C. 渗透测试 / 红队

| 技能 | 功能 |
|---|---|
| `eni-pentest-workflow` | 渗透测试流程 |
| `eni-pentest-tools` | 渗透工具集（最大体量 7.3MB）|
| `eni-pentest-advanced` | 高级渗透技法 |
| `eni-attack-chain` | 攻击链编排 |
| `eni-ctf-orchestrator` | CTF 编排器 |
| `eni-fuzzing-workflow` | 模糊测试（Fuzzing）流程 |
| `eni-firmware-pentest` | 固件渗透测试 |
| `eni-firmware-workflow` | 固件分析流程 |
| `eni-patch-diff-exploit` | 补丁对比 / 漏洞利用 |
| `eni-edr-bypass` | **EDR 绕过 / 免杀**（仅自有靶机研究）|
| `eni-license-security` | 授权/卡密安全设计与逆向审计：在线离线验证、吊销、防回拨 |
| `eni-crack-workflow` | 破解工作流（破解挑战/授权研究，基于保留副本）|
| `eni-llm-security` | LLM 安全 |
| `eni-cloud-container-workflow` | 云/容器安全流程 |
| `eni-code-security-workflow` | 代码安全审计流程 |
| `eni-api-security` | API 安全 |
| `eni-five-edge` | 五维边界渗透 |
| `eni-kali` | Kali 环境引导 |

### D. Web 漏洞细节包（redteam）
> 每个 `eni-redteam-*` 是一个独立的 Web/AD/移动漏洞技术细节包，用于自有资产、SRC 众测、CTF、授权测试。

| 技能 | 覆盖 |
|---|---|
| `eni-redteam-web-detail-pack` | Web 通用漏洞 |
| `eni-redteam-sqli-detail-pack` | SQL 注入 |
| `eni-redteam-xss-detail-pack` | XSS |
| `eni-redteam-ssrf-detail-pack` | SSRF |
| `eni-redteam-ssti-detail-pack` | SSTI 模板注入 |
| `eni-redteam-xxe-detail-pack` | XXE |
| `eni-redteam-cmdi-detail-pack` | 命令注入 |
| `eni-redteam-deserialize-detail-pack` | 反序列化 |
| `eni-redteam-injection-detail-pack` | 注入通用 |
| `eni-redteam-logic-detail-pack` | 逻辑漏洞 |
| `eni-redteam-auth-detail-pack` | 认证绕过 |
| `eni-redteam-access-control-detail-pack`* | 访问控制 |
| `eni-redteam-cors-miscfg-detail-pack` | CORS 配置错误 |
| `eni-redteam-csrf-detail-pack` | CSRF |
| `eni-redteam-open-redirect-detail-pack` | 开放重定向 |
| `eni-redteam-subdomain-takeover-detail-pack` | 子域名接管 |
| `eni-redteam-cache-poison-detail-pack` | 缓存投毒 |
| `eni-redteam-crypto-detail-pack` | 密码学误用 |
| `eni-redteam-file-detail-pack` | 文件处理漏洞 |
| `eni-redteam-network-detail-pack` | 网络层攻击 |
| `eni-redteam-payload-detail-pack` | Payload 构造 |
| `eni-redteam-mobile-detail-pack` | 移动端攻击 |
| `eni-redteam-cloud-detail-pack` | 云平台攻击 |
| `eni-redteam-container-detail-pack` | 容器攻击 |
| `eni-redteam-ad-detail-pack` | 活动目录(AD) |
| `eni-redteam-postex-detail-pack` | 后渗透 |
| `eni-redteam-evasion-detail-pack` | 规避检测 |
| `eni-redteam-recon-detail-pack` / `eni-redteam-recon-intake` | 侦察/信息收集 |
| `eni-redteam-reverse-detail-pack` | 逆向相关红队细节 |
| `eni-redteam-code-audit-detail-pack` | 代码审计 |
| `eni-redteam-cve-lookup` | CVE 查询 |
| `eni-redteam-doctrine` | 红队作战准则 |
| `eni-redteam-clickjacking-detail-pack` | 点击劫持 |

### E. API / 浏览器 / 自动化

| 技能 | 功能 |
|---|---|
| `coldbrew-api-reverse` | 前端签名/HAR/鉴权链路/加密参数还原 |
| `coldbrew-identity` | ColdBrew 身份体系 |
| `coldbrew-native-reverse` | 原生层冷萃逆向 |
| `coldbrew-protocol-reverse` | 协议逆向 |
| `eni-browser-automation` | 浏览器自动化（Playwright） |
| `eni-browser-research-workflow` | 浏览器研究流程 |
| `eni-burp-mcp` | Burp 套件 MCP 集成 |
| `eni-scraper-workflow` | 数据采集/爬虫流程 |
| `eni-diagram` | 图表/架构图 |
| `eni-docs` | 文档生成 |

### F. 方法论 / 流程 / 平台

| 技能 | 功能 |
|---|---|
| `eni-architecture-workflow` | 架构清单/组件边界/威胁评审 |
| `eni-case-lab` | 案例实验室 |
| `eni-field-journal` | 现场日志/研究笔记（235KB）|
| `eni-unified-router` | eni-solo 确定性路由器 |
| `eni-universal-workflow` | 通用流程编排 |
| `eni-software-workflow` | 软件开发流程 |
| `eni-supply-chain` / `eni-supply-chain-assurance-lane` | 供应链安全/保障 |
| `eni-api-assurance-lane` | API 保障 |
| `eni-github-workflow-hub` | GitHub Actions 工作流 |
| `eni-cf-security-lab-router` | 实验室路由 |
| `codex-gpt55-instructions-deploy` | GPT-5.5 技术文档资料集（资料查阅）|

> *注：`eni-redteam-access-control-detail-pack` 在本包中可能未单独收录，请以仓库实际目录为准。

---

## 使用边界

本技能库内容来自开源/授权逆向资料整理。**请严格遵守**：

1. **仅限**以下场景使用：自有程序/资产、书面授权的渗透测试、SRC 众测、CTF 竞赛、隔离沙箱、防御性安全研究。
2. **禁止**用于：未授权入侵、窃取密钥/数据、绕过他人商业授权、对第三方服务实施未授权攻击、制作/传播恶意软件。
3. 部分技能（`eni-edr-bypass`、`eni-crack-workflow`、`eni-license-security`、`eni-game-cheat-*`、`eni-cf-security-lab-router`、`eni-redteam-*`）标注为**越权/破解/作弊类**，仅在上述授权边界内使用。
4. 涉及别人 API key、验证凭据的内容（原包中携带的 DeepSeek token 等）已**全部剔除**，本仓库不含任何真实凭据。
5. 你最终对自己的行为负责。小羊助手只协助合法授权的技术研究与开发。