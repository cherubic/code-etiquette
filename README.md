# code-etiquette

我个人的代码习惯规范，会结合目前已有的规范文档以及相关工具。

## commit

1. 相关规范
    - [约定式提交规范](https://www.conventionalcommits.org/zh-hans/v1.0.0/#%e7%ba%a6%e5%ae%9a%e5%bc%8f%e6%8f%90%e4%ba%a4%e8%a7%84%e8%8c%83)
    - [语义版本规范2.0.0](https://semver.org/lang/zh-CN/)
    - [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt)

2. 相关工具
    - git hook: [website](https://git-scm.com/book/zh/v2/%E8%87%AA%E5%AE%9A%E4%B9%89-Git-Git-%E9%92%A9%E5%AD%90)；git操作的hook，分别有 `pre-commit`(提交前), `prepare-commit-msg`  (编辑提交信息前), `commit-msg`(编辑提交信息后), `pre-receive`(推送接收到信息前), `update`(更新引用前，一般用于服务端触发), `pre-push`(推送前), `post-update`(引用更新后)
    - commitlint: [website](https://commitlint.js.org/#/), [github](https://github.com/conventional-changelog/commitlint)；校验提交消息的工具
    - Commitizen: [website](http://commitizen.github.io/cz-cli/), [github](http://commitizen.github.io/cz-cli/)；提交代码时强制执行规范化的提交消息格式
    - cz-customizable(可选): [github](https://github.com/leoforfree/cz-customizable)；提交代码时强制执行规范化的提交消息格式
    - husky: [website](https://typicode.github.io/husky/#/), [github](https://github.com/typicode/husky)；git hook管理工具


3. 相关脚本
    - commit-init.sh (Linux/Mac脚本)
    - commit-init.ps1 (Windows脚本)

4. 如何使用
    1. 首先必须预先安装git，node命令以及相关工具
    2. 下载对应脚本，终端进入需要初始化的项目后执行脚本即可。例： `wget <bash-url> && cd ~/myproject && bash ~/commit-init.sh`