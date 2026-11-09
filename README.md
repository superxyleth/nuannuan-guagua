# 暖暖和瓜瓜 · DeepSeek Harness 伙伴素材

暖暖戴着橙色仓鼠兜帽，瓜瓜抱着一颗瓜子。素材包保留了两位角色的 9 组动画和 16 个视线方向帧，供支持 Codex v2 图集的 DeepSeek Harness（DSH）Web 伙伴适配器读取。

## 1. 下载并校验

打开 [v1.0.0 发布页](https://github.com/superxyleth/nuannuan-guagua/releases/tag/v1.0.0)，在 **Assets** 下下载 `Nuannuan-Guagua-DSH-assets-v1.0.0.zip`。下载无需登录 GitHub。

在 ZIP 所在目录打开 PowerShell，运行下面的命令：

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath './Nuannuan-Guagua-DSH-assets-v1.0.0.zip'
```

预期 SHA-256 值如下，大小写均可。

```text
61b2fb3e2c7c8e0c0d2c86c988be3975d7bca52e0edbf1d0abf2cea78e0cdd4c
```

校验通过后解压。包内的 `SHA256SUMS` 还列出了图集和清单各自的校验值。

## 2. 导入 DSH

1. 确认公司允许下载此素材包，并且 DSH Web 已启用经公司批准、支持 Codex v2 图集和文件夹导入的伙伴适配器。
2. 打开适配器的伙伴设置，选择解压后的 `nuannuan-guagua.codex-pet` 文件夹。该文件夹内的 `pet.json` 指向同目录的 `spritesheet.webp`。
3. 在伙伴列表中选择「暖暖和瓜瓜」。用虚构内容测试待机、工作和等待状态。失败动画和指针跟随的触发取决于适配器版本。

素材包只含透明 WebP 图集、JSON 清单、校验值和说明。模型连接和任务权限由 DSH 及公司环境管理。使用公司资料前，确认公司批准的模型入口和数据处理范围。

## 文件一览

| 文件 | 用途 |
| --- | --- |
| `nuannuan-guagua.codex-pet/pet.json` | 伙伴名称、描述、图集文件名和 v2 版本声明 |
| `nuannuan-guagua.codex-pet/spritesheet.webp` | 1536 × 2288 透明 WebP 图集，无损保留已验证 PNG 的像素 |
| `SHA256SUMS` | 图集与清单的 SHA-256 校验值 |
| `README.md` | 素材包内的简要导入说明 |
