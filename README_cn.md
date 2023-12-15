# chatwoot

```bash
# 设置代理
export http_proxy=http://127.0.0.1:10818
export https_proxy=http://127.0.0.1:10818
# node版本
nvm use 20.0.0
# https://www.chatwoot.com/docs/contributing-guide/project-setup
# clone the repo and cd to chatwoot dir
git clone https://github.com/pengjinning/chatwoot.git
cd chatwoot
# 安装依赖
make burn
# 设置数据库+redis密码
cp .env.example .env
# 生成数据库
# run db migrations
make db
# fireup the server
foreman start -f Procfile.dev
# 打开浏览器，管理后台地址
# http://localhost:3000
# 管理员密码
user name: john@acme.inc
password: Password1!
# 超级管理员后台
# http://localhost:3000/super_admin/users
# 访客端地址
# http://localhost:3000/widget_tests
# http://localhost:3000/widget_tests?setUser=true
# api地址
# http://localhost:3000/swagger

```
