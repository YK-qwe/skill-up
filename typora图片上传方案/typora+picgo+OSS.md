<!--阿里云OSS以及Github作免费图床都不好用，现使用相对路径-->

# typora官网

中文站：https://typoraio.cn/

激活码：4ZRQQH-QXF4PJ-MQ3S6H-VXZQY5

笔记github托管：https://github.com/YK-qwe/typora

# PicGo

https://github.com/Molunerfinn/picgo/releases?page=1

版本：2.3.1

PicGo-Setup-2.3.1-x64.exe

# 阿里云OSS

https://home.console.aliyun.com/

- AccessKey ID：LTAI5tN1pfKYjMzQmRVrh8cX
- AccessKey Secret：XOZc6wTHxlqvuFypRk3L9O4p4s6yM6
- 登录密码：{5dMYTKhO|ei$Ct4|GE1zBuO7mNQnlga

# 各软件配置

作者：小逸Maverick
链接：https://juejin.cn/post/7311630480335814706
来源：稀土掘金
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

## 阿里云OSS

### 1.创建Bucket

进入“管理控制台” ==> 创建OSS Bucket ==> 

- **Bucket 名称**：给你的 Bucket 取名
- **地域**：选择“有地域属性”，然后选择地域。
- **存储类型**：选择“标准存储”即可。
- **存储冗余类型**：推荐选择“本地冗余存储”。
- **读写权限**：一定要选择“公共读”，否则平台无法通过公网访问 Bucket 中的内容。

其他选项推荐默认即可。

### 2.创建子用户AccessKey

右上角用户界面进入“AccessKey”管理界面 ==> 选择"开始使用子用户AccessKey" ==> 创建用户 ==>

输入“登录名称”和“显示名称”，**勾选“控制台访问”和“OpenAPI 调用访问”** ，其他默认即可 ==> 

将“AccessKey ID”和“AccessKey Secret”复制并粘贴到记事本上，待会要用到这些信息。（**一定要复制，否则页面关闭后就没法再获取这些信息了！** ） ==> 然后选中该用户，点击“添加权限”，为子用户添加“管理 OSS 权限”

### 3.授予子用户Bucket管理权限

回到 Bucket 页面，找到“权限控制”面板，点击“Bucket 授权策略”，新增授权 ==>

- **授权用户**：选择刚刚创建的子账户。
- **授权操作**：选择“完全控制”。

其他选项默认即可。

## PicGo配置

图床设置 ==> 阿里云OSS

- **设定 KeyId**：将刚刚复制的“AccessKey ID”粘贴到这里。

- **设定 KeySecret**：将刚刚复制的“AccessKey Secret”粘贴到这里。

- **设定 Bucket**：填入“存储空间名称”（Bucket 名称）。

- **设定存储区域**：如果刚刚的“地域”选择的是杭州，这里就填“oss-cn-hangzhou”。如果是其他地域，就将这里的“hangzhou”替换为其他地域拼音名称即可。

![image-20241011090754842](https://picgoimg-typora.oss-cn-hangzhou.aliyuncs.com/202410110907881.png)

## Typora配置

文件 ==> 偏好设置 ==> 图像

![image-20241011090956822](https://picgoimg-typora.oss-cn-hangzhou.aliyuncs.com/202410110909862.png)