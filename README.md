# -json-maze.json
此脚本是适用于项目x-glacier GenerativeAgentsCN，可以将自义定地图转成ai能理解的maze文件


# TiledToMaze (Tiled地图转Maze工具)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

一个简单高效的工具，将Tiled编辑器导出的JSON地图文件转换为Maze格式和空间树结构。支持多线程处理和实时进度显示，适用于游戏开发中的地图处理。

## 功能特点

- ✅ 支持从Tiled导出的JSON地图文件转换
- ✅ 一键生成标准Maze格式文件
- ✅ 自动构建空间树结构
- ✅ 多线程处理大型地图文件
- ✅ 实时进度条显示转换状态
- ✅ 用户友好的GUI界面

## 安装说明

### 环境要求
- Python 3.6+
- tkinter (通常随Python安装)

### 安装步骤

1. 克隆仓库到本地
```bash
git clone https://github.com/你的用户名/TiledToMaze.git
cd TiledToMaze
```

2. 运行程序
```bash
python json地图转换maze脚本3y9r.py
```

## 使用方法

1. 启动程序
2. 点击"选择文件"按钮，选择Tiled导出的JSON地图文件
3. 选择输出目录
4. 设置Maze文件和空间树文件的名称
5. 点击"一键转换"按钮开始转换
6. 查看日志区域获取转换进度和结果

## 支持的图层格式

工具支持两种命名格式的图层：

1. 传统格式:
   - `sector-xxx`: 扇区层
   - `arena-xxx`: 区域层
   - `object-xxx`: 物体层

2. 数字前缀格式:
   - `1xxx`: 对应扇区层
   - `2xxx`: 对应区域层
   - `3xxx`: 对应物体层

## 项目结构

- `convert_tiled_to_maze()`: 将Tiled JSON地图转换为Maze格式
- `convert_maze_to_tree()`: 将Maze数据转换为空间树结构
- `build_location_hierarchy()`: 构建地点层级关系
- `TiledToSpatialTreeConverter`: GUI界面类

## 常见问题

**Q: 如何调整碰撞图层设置?**  
A: 在代码中修改 `collision_tiles` 数组的值。

**Q: 转换大型地图时会不会卡顿?**  
A: 程序使用了多线程处理，将耗时操作放在后台执行，界面不会卡顿。

**Q: 支持哪些Tiled地图格式?**  
A: 目前支持Tiled导出的JSON格式地图文件。

## 贡献指南

欢迎提交问题和改进建议！如需贡献代码，请遵循以下步骤：

1. Fork 本仓库
2. 创建您的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交您的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个 Pull Request

## 许可证

本项目采用 MIT 许可证 - 详情请查看 [LICENSE](LICENSE) 文件

## 联系方式

如有任何问题或建议，请通过 GitHub Issues 联系我们。

---

希望这个工具能帮助您简化游戏开发中的地图处理工作！
