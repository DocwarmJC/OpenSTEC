# STEC规则参考

---

STEC的命令均以"@"开头，以";"结尾，用法为：

```
@command;
```

若要输出"@"字符则输入"@@"即可。
可根据功能需要做出其他扩展。

#### 指令参考v0.1

---

> 1. 变量与使用方法
> 2. @set;
> 3. @reset;
> 4. @sleep;

1.变量：
    变量用\$+()使用，如`$(var)`；赋值则为`@$(var):var`，或者这样：`@$(var):$(var_1)`，变量命名规则为可以用字母数字下划线且数字不能作为开头。
命令使用方法：
    "@command[:var];"是命令的使用方法，多个参数用","隔开，剩下命令以后会讲。

2.`@set;`
    能够控制输出的字体信息，使用方法为："@set:var;"，有三个参数fore、back和te；

    新的`@set;`将会覆盖之前的`@set;`参数。

> 1.fore参数（前景色）
> 
> > black
> > 
> > red
> > 
> > green
> > 
> > yellow
> > 
> > blue
> > 
> > purple
> > 
> > cerulean
> > 
> > white
> 
> 2.back参数（背景色）
> 
> > black
> > 
> > red
> > 
> > green
> > 
> > yellow
> > 
> > blue
> > 
> > purple
> > 
> > cerulean
> > 
> > white
> 
> 3.ts参数（文本特效可叠加）
> 
> > strong
> > 
> > italic
> > 
> > underline
> > 
> > glittery
> > 
> > hide

3.`@reset;`

    `@reset;`能够重置`@set;`的文字效果，使其重置为默认的显示方式；

4.`@sleep;`

    `@sleep;`能够使文本输出暂停其使用方法为`@sleep:time;`,即使文字输出time秒。
