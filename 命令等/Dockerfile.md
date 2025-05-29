# 内网镜像缺少某个组件时
- Docker file制定pip源
- [x] RUN mkdir ~/.pip && wget -O ~/.pip/pip.conf http://100.6.60.13/pip.conf
- RUN pip install
# .gitignore怎么写
# Git 相关
.git
.gitignore
```
# Python 缓存和编译文件
__pycache__/
*.pyc
*.pyo
*.pyd

# Python 构建/打包产物
build/
dist/
*.egg-info/
pip-wheel-metadata/

# 虚拟环境目录
.venv/
venv/
env/

# IDE 和操作系统特定文件
.vscode/
.idea/
*.swp
*~
.DS_Store
Thumbs.db

# 测试相关
.pytest_cache/
.coverage
htmlcov/

# 文档构建
docs/_build/

# 本地设置/密码文件 (绝不应该进入镜像)
*.env
local_settings.py
secrets.*
*.pem
*.key

# 日志文件
*.log

# 其他常见排除项
notebooks/ # 如果有 Jupyter notebooks 且不需要它们
data/ # 如果有大量本地数据
*.zip
*.tar.gz
```
