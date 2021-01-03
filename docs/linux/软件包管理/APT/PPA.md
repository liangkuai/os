# PPA

> PPA 全称为 Personal Package Archives（个人软件包档案），是 Ubuntu Launchpad 网站提供的一项服务，当然不仅限于 Launchpad 。它允许个人用户上传软件源代码，通过 Launchpad 进行编译并发布为二进制软件包，作为 apt/新立得源供其他用户下载和更新。在 Launchpad 网站上的每一个用户和团队都可以拥有一个或多个PPA。
>
> 通常 PPA 源里的软件是官方源里没有的，或者是最新版本的软件。相对于通过 Deb 包安装来说，使用 PPA 的好处是，一旦软件有更新，通过sudo apt-get upgrade这样命令就可以直接升级到新版本。


### 通过PPA源安装软件

1. 在 [launchpad.net](https://launchpad.net/ubuntu/+ppas) 上搜索软件名称，通过以下命令将 PPA 源添加到 `/etc/apt/sources.list.d` 目录

    ```bash
    sudo add-apt-repository ppa:xxx
    ```

2. 更新软件源

    ```bash
    sudo apt update
    ```

3. 安装软件

    ```bash
    sudo apt install xxx
    ```
