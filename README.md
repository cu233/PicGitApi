<div align="center">


## 本项目fork自[AUXPI](https://github.com/aimerforreimu/auxpi)

## 1.分发原理

![流程图](https://ae01.alicdn.com/kf/HTB1ikH2TY2pK1RjSZFs761NlXXaN.png)


## 2.代码组织

```text
.
├── LICENSE
├── README.md
├── auxpiAll
├── bootstrap
├── build
├── build.sh
├── conf
├── controllers
├── install.sh
├── log
├── main.go
├── middleware
├── models
├── pem
├── resource
├── routers
├── server
├── static
├── tests
├── tools
├── utils
└── views

```



**成功上传返回**

```json
{
    "code": 200,
    "msg": "上传成功",
    "data": {
        "name": "Snipaste_2018-08-28_01-17-58.png",
        "url": "https://img04.sogoucdn.com/app/a/100520146/0dcb98aadb59c6b29dc0832eb7cc094a"
    }
}

```

```json
{
    "code": 200,
    "msg": "上传成功",
    "data": {
        "name": "Snipaste_2018-08-28_01-17-58.png",
        "url": "https://i.loli.net/2018/11/05/5be038b1b4af6.png"
    }
}
```

**失败返回值**

上传出错返回值

```json
{
    "code": 500,
    "msg": "上传失败"
}
```

API 未开启返回值

```json
{
    "code": 405,
    "msg": "Method not allowed"
}
```
 Token 验证失败返回值
 
```json
{
    "code": 403,
    "msg": "Forbidden"
}
```

选择文件为空返回值

```json

{
    "code": 500,
    "msg": "No files were uploaded."
}

```

文件太大返回值

```json

{
    "code": 500,
    "msg": "File is too large."
}

```



## 致敬
[@ astaxie](https://github.com/astaxie) (beego)

[@ PanJiaChen](https://github.com/PanJiaChen) (vue-element-admin)

[@ metowolf](https://github.com/metowolf/upimg-cli) (upimg-cli)

[@ wisp-x](https://github.com/wisp-x) (lsky-pro)

[@ aimerforreimu](https://github.com/aimerforreimu)(auxpi)

