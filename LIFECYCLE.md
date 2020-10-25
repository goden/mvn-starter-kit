# Maven生命週期

Maven的生命週期定義一個項目建構與發佈的過程. Maven有三個標準的生命週期：

- **clean**，清除建置項目
- **default/build**，建置項目的建構與部署
- **site**，建置項目文件的產出

![maven-0001](pic/maven-0001.png)

一個插件目標代表一個特定的任務（比構置階段更為精細），這些目標可能被綁定0 ~ n個階段。零綁定的目標可以在生命週期之外通過直接呼叫執行。這些目標的執行順序取決於呼叫的目標和執行建置階段的順序。

例如，考慮下面的命令：

`clean` 和 `pakage` 是構建階段，`dependency:copy-dependencies` 是目標。clean階段先執行，接下來dependency:copy-dependencies目標被執行，最後才輪到package階段。

```bash
$ mvn clean dependency:copy-dependencies package
```