# ResearchKit（公开镜像）

本仓库为 **公开（public）** 仓库，仅用于让新成员快速获取团队工具，**不包含任何明文源码**。

## 仓库里有什么

- `researchrepo_template.zip` —— 项目模板（加密归档）
- `REF_aisec.zip` —— 参考文献库 `REF_aisec.bib`（加密归档）
- `SRC/` —— **未加密的源文件，已被 `.gitignore` 排除，不会出现在本仓库中**

## 如何使用

1. 克隆本仓库：
   ```bash
   git clone https://github.com/nice-grp/ResearchKit.git
   cd ResearchKit
   ```
2. 用团队共享的**解密密码**解压每个归档（密码请向团队负责人私信获取，**不要**写在公开 Issue / 评论里）：
   ```bash
   unzip -P <解密密码> researchrepo_template.zip -d .
   unzip -P <解密密码> REF_aisec.zip -d .
   ```
   也可使用 7-Zip / The Unarchiver / Keka 等支持加密 zip 的图形化工具。

解压后得到的目录结构与本地 `SRC/` 一致，可直接作为工作副本。

## 安全说明

- 本仓库历史中**从未包含未加密的敏感内容**；真正的源文件只保留在本地 `SRC/` 与私有备份中。
- 当前归档使用 zip 传统加密（ZipCrypto）。它对"防止外人随手浏览"足够，但传统 zip 加密强度有限；若需更强保护，建议改用 7-Zip AES-256 重新打包（见团队内部说明）。
- **切勿把解密密码提交进本仓库或写在公开位置。**
