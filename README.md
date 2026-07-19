# ArchDomain 筑域国际 — 企业品牌官网

建筑全产业链一站式解决方案品牌站。

## 🚀 GitHub Pages 部署指南

### 第一步：添加 SSH 公钥

复制下面的公钥：

```
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIC3ML3sP5Tu6FEu/wckThB788GF4EXeMdF/pmMsMDi0m archdomain-deploy
```

1. 打开 https://github.com/settings/keys
2. 点击 **New SSH key**
3. Title 填：`ArchDomain Deploy`
4. Key 粘贴上方公钥
5. 点击 **Add SSH key**

### 第二步：创建 GitHub 仓库

1. 打开 https://github.com/new
2. Repository name 填：`archdomain-site`
3. 选择 **Public**
4. **不要勾选**任何初始化选项
5. 点击 **Create repository**

### 第三步：一键部署

在 Git Bash 中运行：

```bash
cd /f/archdomain-site
bash deploy-github.sh
```

脚本会自动完成所有操作，部署到 `https://你的用户名.github.io/archdomain-site`

## 📁 文件结构

```
F:/archdomain-site/
├── index.html          # 网站主文件（中英双语）
└── deploy-github.sh    # GitHub Pages 部署脚本
```

## 🛠 自定义修改

如需修改公司名称、联系方式、业务描述等，直接编辑 `index.html` 中的对应内容即可。

修改后重新运行 `bash deploy-github.sh` 更新网站。
