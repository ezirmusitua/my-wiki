## 尝试 Travis-CI  
1. 在线的  
2. 分布式  
3. 持续集成  
4. 构建及测试  
5. Github 项目  
6. 支持多种语言  
7. 开源的  

### 官方教程  
使用 Github 账号登陆  

#### 激活 Github repo  
在[这里](https://travis-ci.org/profile/)进入你的 profile 中激活 Github Repo  

#### 为 repo 增加 .travis.yml 文件  
在[这里](查看相关语言的`yml`文件编写方式)  

#### 首次 git-push 构建  
将 .travis.yml commit & push 到 Repo 中

* commit & push  
* [GITHUB Repo Setting](https://github.com/ezirmusitua/<your-repo-name>/settings) -> Webhooks & Services -> Travis CI -> Test Services 

### 实践教程  
#### Javascript
```  
language: node_js  
node_js:
    - "5.11"  

before_script:  
    - npm install  

script:
    - npm start
```  
针对 NodeJS 类型的项目  
指定语言/指定版本/在运行`script`之前做什么/运行`script`  

#### Python  
```  
language: python  
python: 
    - "2.7"

install: "pip install -r requirements.txt"

script: "python main.js"
```  
同上


