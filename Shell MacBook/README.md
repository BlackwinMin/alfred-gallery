本动作用于给截图套壳，需先行安装 imagemagick。

![title](Shell%20MacBook.gif)

可自行增减素材。以添加自定义素材为例，操作步骤为：

1. 将素材与 LaunchBar 脚本置于统一目录下
2. 在调用提示框部分的机型列表 `list_1` 后添加机型，名称与素材文件名保持一致
3. 在 if 判断部分增加套壳代码

```
elif [ "$shellImage" = "机型名称" ]; then
        composite "-geometry" "边距参数" "$f" "$shellImage".png "$newFile"
```