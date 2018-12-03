# 使用SASS编写可维护性的CSS

每次使用SASS 编写CSS的时候除了嵌套感觉没有用到其它的更多API和语法。而深层的嵌套使得维护成本越来高更加难已维护，这段时间正好有空所以更加深入的学习一些SASS的 API和语法。

## 关键词的重新认识

###  `&` 连体符
说到`&`用到最多的肯定是在伪类上
```scss
.link {
    color : #ccc;
    &:hover {
        color:#f00;
    }
}
```
多类
```scss
.link{
    color:#ccc;
    &.is-active{
        color:#f00;
    }
}
```

2. %


## 参考链接 
[Sass编写规范](https://sass-guidelin.es/zh/)