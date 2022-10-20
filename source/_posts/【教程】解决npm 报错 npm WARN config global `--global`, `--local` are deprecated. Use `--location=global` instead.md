# 问题描述
只要在控制台执行npm，不论有没有参数，都会有此警告：
``npm WARN config global `--global`, `--local` are deprecated. Use `--location=global` instead.``

# 解决方案

### 以管理员身份打开cmd并执行以下命令
```bash
npm install -g npm-windows-upgrade
```

### 以管理员身份打开Windows Power Shell并执行以下命令
  在出现提示后输入 Y
```shell
set-ExecutionPolicy RemoteSigned
```

### 在Windows Power Shell中执行以下命令
  执行后提示选择版本，使用键盘右边的方向键选择
```shell
npm-windows-upgrade
```

- 查看npm版本
  
> npm -v
  
- 选择相应版本后按下回车

---

>参考来源：CSDN:[颜值与实力并存源](https://blog.csdn.net/SOLar7SysteM/article/details/125892594)