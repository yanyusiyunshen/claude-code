# claude-code创建，连接Deepseek（Linux环境）

## conda的安装

官网下载安装

```
https://anaconda.org/
```

## 创建虚拟环境

```
# 创建虚拟环境
conda create --name claude_code python 

# 查看虚拟环境
conda env list 

# 激活虚拟环境
conda activate claude_code 

# 退出虚拟环境
conda deactivate 
```

## node.js的安装

进入虚拟环境后

```
# 安装node.js
conda install -c conda-forge nodejs

node --version  

# 查看相应版本号
npm --version    
```

## claude-code的安装

```
#安装Claude-code
npm install -g @anthropic-ai/claude-code # 可能很慢

# 安装完成查看版本号
claude --version 
```

## ccswitch安装

```
# 安装
npm install -g claude-sw

# 初始化配置（交互式设置各平台 API Key）
ccs init

# 切换提供商
ccs aliyun          # 切换到阿里百炼
ccs deepseek        # 切换到 DeepSeek
ccs zhipu glm-5     # 切换到智谱 GLM

# 查看状态
ccs current         # 当前配置
ccs list            # 所有可用提供商

# 仅切换模型（保持提供商）
ccs model qwen-max
```

也就可以去官网下载

```
https://github.com/farion1231/cc-switch/releases
```

配置api key和模型等信息



## vscode连接

打开deepseek开放平台配置信息获取api key

在插件中搜索claude code安装
