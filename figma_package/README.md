# Figma 可导入设计包（MVP）

你可以把 `screens/*.svg` 直接拖进 Figma，系统会自动变成可编辑图层。

## 先说结论（避免踩坑）
- ✅ **能直接拖进 Figma**：`.svg`（本包里的 `screens/*.svg`）。
- ⚠️ **不能直接当画面拖进去**：`.md` 文档（`BRD.md` / `PRD.md` / `UI_CONCEPT_FIGMA.md`）与 `.json`（`design-tokens.json`）。
- 如果要在 Figma 看文档内容：请把文档内容复制到 Figma 的 Text 图层，或粘到 FigJam。


## 你现在这个问题：看到的是链接，怎么拖？
是的，**如果你现在在网页里看到的是仓库文件链接**，需要先把文件下载到本地，才能拖进 Figma。

### 场景 A：你在 GitHub 网页看仓库
1. 点仓库右上角 `Code` → `Download ZIP`。
2. 解压 ZIP。
3. 进入解压后的 `figma_package/screens/` 目录。
4. 把 5 个 `.svg` 文件直接拖进 Figma。

### 场景 B：你在代码编辑器/本地文件夹（能看到真实文件）
- 直接打开 `figma_package/screens/`，选中 `.svg` 拖入 Figma 即可，不用额外下载。

### 场景 C：只想导入单个页面
- 在 GitHub 点开某个 `*.svg` 文件，点击 `Download raw file` 保存到本地，再拖进 Figma。

## 包含内容
- `screens/01_home.svg` 首页（记录）
- `screens/02_upload.svg` 上传页
- `screens/03_result.svg` 结果页
- `screens/04_analysis.svg` 分析页
- `screens/05_profile.svg` 我的页
- `tokens/design-tokens.json` 设计 Token 草案

## 导入步骤（2 分钟）
1. 打开 Figma 文件（建议新建页面 `03_HiFi_Screens`）。
2. 打开本地目录 `figma_package/screens/`。
3. 选中 5 个 `.svg` 文件，直接拖入 Figma 画布空白区域。
4. 全选导入后的画板，执行 **Frame selection**，并命名为：
   - `iOS_Home_Default_v1`
   - `iOS_Upload_Default_v1`
   - `iOS_Result_Default_v1`
   - `iOS_Analysis_Default_v1`
   - `iOS_Profile_Default_v1`
5. （可选）在 Figma Variables/Styles 里，按 `tokens/design-tokens.json` 手动建立颜色和文字样式。

## 文档怎么用（不是拖拽）
- `BRD.md`：给产品/业务评审用。
- `PRD.md`：给设计/研发对齐需求用。
- `UI_CONCEPT_FIGMA.md`：给设计师按清单出图与连线用。

建议做法：在 Figma 右侧开一个注释区，复制 `UI_CONCEPT_FIGMA.md` 的“页面要求”段落作为设计注释。

## 常见问题
- 看不到中文字体：把字体替换为 Figma 可用字体（如 Inter / PingFang SC）。
- SVG 被当成一整张图：进入图层后右键 **Ungroup** 或 **Flatten 还原前版本**。
- 拖拽失败：用 Figma 顶部菜单 `File > Place image...` 选择 SVG 再导入。

## 说明
- 这是 UI 概念图，不是最终视觉稿。
- 如你愿意提供 Figma 文件链接（并授权编辑），我可以继续按此包做下一版高保真与原型连线说明。
