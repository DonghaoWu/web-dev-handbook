8/16:

1. set up a ssh key to github.

```bash
$ ssh-keygen -o // 创建 ssh key，然后一直按 enter。

$ cat /Users/donghao/.ssh/id_rsa.pub // 调出 ssh 字符串。
```

- 最后登陆 Github，在 setting => SSH keys and GPG keys 一栏 => create new SSH keys => `填写 title 和粘贴 ssh 字符串。`

- 注意，设置了 ssh 方式之后，每次创建或者下载 repo 都要手动选择 SSH 方式。