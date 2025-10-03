# project-auto-backup

project auto backup by git-autosync (xscript

## Quick Start / 快速开始

> run in project root directory

**step0: get this project / 获取项目**

```bash
git clone https://github.com/Sunrisepeak/project-auto-backup.git
```

**step1: install deps(git-autosync) & auto config / 安装依赖并自动配置**

```
xlings install
```

> - [download xlings](https://xlings.d2learn.org/documents/quick-start/one-click-install.html)
> - default sync project when 01:00 in everyday / 默认每天凌晨1点同步

**step2: add your git url to `.git-autosync` / 添加git仓库url到`.git-autosync`文件**

- support https and ssh

**step3: manual sync / 手动同步 (可选)**

```
git-autosync sync
```

## More Features / 更多功能

**add sync task (option/default) **

```bash
git-autosync add . --time "* * * 1 *"
```

- `--tmie`: [Week Month Day Hour Minute]
  - `* * * 1 *`: when 01:00 for everyday
  - `Mon * * 1 *`: when Mon's 01:00 for every week

**get task list or log**

```bash
git-autosync log
git-autosync list
```

## Other

- xlings: https://github.com/d2learn/xlings
- git-autosync: https://github.com/d2learn/xim-pkgindex/tree/main/pkgs/g/git-autosync.lua