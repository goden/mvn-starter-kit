# Maven POM

POM ( Project Object Model ) 是 Maven 所參考的XML主檔，包含了項目的模組版本，宣告項目相依性，定義執行任務…等，以下是POM檔主要的基本架構。

```xml
<project xmlns = "http://maven.apache.org/POM/4.0.0"
    xmlns:xsi = "http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation = "http://maven.apache.org/POM/4.0.0
    http://maven.apache.org/xsd/maven-4.0.0.xsd">
 
    <!-- 模組版本 -->
    <modelVersion>4.0.0</modelVersion>
  
    <!-- 唯一識別標幟，通常指的是公司或組織，配置路徑也是由此而來， 如com.companyname.project-group，maven會將專案項目打包成jar或war檔包後放置於本機目錄：/com/companyname/project-group -->
    <groupId>com.companyname.project-group</groupId>
 
    <!-- 项目的唯一ID，一个groupId下面可能多個项目，就是靠artifactId來辨別 -->
    <artifactId>project-name</artifactId>
 
    <!-- 版本號通常預設是會帶有snapshot關鍵字 -->
    <version>1.0</version>
</project>
```

每個POM檔皆會含括以下項目：

| 元素         | 描述                                                         |
| ------------ | ------------------------------------------------------------ |
| project      | POM的根節點                                                  |
| modelVersion | 4.0.0為標準值.                                               |
| groupId      | 泛指一個組織或公司所屬專案項目的唯一標幟，例：`com.mycompany.project`。groupId也代表在maven repository中的目錄結構 |
| artifactId   | 代表此artifact的識別ID，在此指的是函式庫名稱。`artifactId`與`groupId`的搭配通常指的是在repository中，按groupId所目錄結構所指向的函式庫名稱。例：`com.mycompany.project.library` |
| version      | 指的是artifact的版號。例：`com.mycompany.project.library:1.0` |

