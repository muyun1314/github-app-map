# GitHub App Map

GitHub 软件映射库 - 为 GitHub Updater 提供「程序名 → GitHub 仓库」的公共映射数据。

## 用途

当 GitHub Updater 扫描你电脑上的软件时，会自动查询这个映射库，把 exe 文件名匹配到对应的 GitHub 仓库，从而自动获取版本更新信息。

## 文件说明

- `apps.json` — 主映射数据

## 贡献方式

### 方式一：通过 GitHub Updater 客户端

在软件中点击「贡献映射」按钮，自动提交。

### 方式二：手动提交

Fork 本仓库，在 `apps.json` 中添加映射条目，提交 PR。

### 映射条目格式

```json
{
  "exe_name": "yt-dlp.exe",
  "product_names": ["yt-dlp"],
  "repo": "yt-dlp/yt-dlp",
  "main_exe_path": "yt-dlp.exe",
  "install_type": "Portable",
  "contributor": "your-username",
  "contributed_at": "2025-01-01T00:00:00Z"
}
```

## License

MIT
