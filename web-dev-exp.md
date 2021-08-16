8/16:

1. `Set up a SSH way to github.`

```bash
$ ssh-keygen -o // 创建 ssh key，然后一直按 enter。
$ cat /Users/donghao/.ssh/id_rsa.pub // 调出 ssh 字符串。
```

- 最后登陆 Github，在 setting => SSH keys and GPG keys 一栏 => create new SSH keys => `填写 title 和粘贴 ssh 字符串。`

- 注意，设置了 ssh 方式之后，每次创建或者下载 repo 都要手动选择 SSH 方式。

2. `Set up a http way to github.`

```bash
$ brew tap microsoft/git
$ brew install --cask git-credential-manager-core
```

- 然后登陆 Github，在 setting => Developer setting 一栏 => Personal access tokens => Generate new token => 填写权限 => 复制生成的 token。

- 在对应所在的 repo terminal 中，

```bash
$ git add .
$ git commit -m'my commit.'
$ git push
```

- 弹出窗口，选择 token 登陆，粘贴 token 即可。
