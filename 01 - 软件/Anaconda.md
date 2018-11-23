# Anacond

- Anacond是一款Python的虚拟环境管理器,并且具有安装包管理功能。

## 镜像源
- 因为Anacond的默认镜像源是国际镜像源，在国内使用非常的不稳定，常常导致插件安装失败，所以在安装插件之间更换Anacond安装源为国内安装源
- 推荐使用中国科技大学的镜像站
    ```
    https://mirrors.ustc.edu.cn/anaconda/
    ```

### 更换镜像源

- 添加USTC仓库镜像:
    ```
    conda config --add channels https://mirrors.ustc.edu.cn/anaconda/pkgs/free/
    conda config --add channels https://mirrors.ustc.edu.cn/anaconda/pkgs/main/
    conda config --set show_channel_urls yes
    ```
- 添加Conda 附加库:
  - Conda Forge
    ```
    conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/conda-forge/
    ```
  - msys2
    ```
    conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/msys2/
    ```
  - bioconda
    ```
    conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/bioconda/
    ```
  - menpo
    ```
    conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/menpo/
    ```

- 查看配置是否生效
    ```
    conda info
    ```
## 指令
- 创建虚拟环境,xxx = 虚拟环境的名称
    ```
    conda create -n xxx python=3.6 -y
    ```
- 显示Anaconda安装包
    ```
    conda list
    ```
- 显示Anaconda虚拟环境
    ```
    conda env list
    ```