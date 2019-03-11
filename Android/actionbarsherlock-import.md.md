#在module的build.gradle文件中设置dependencies，如下：

        implementation 'com.actionbarsherlock:actionbarsherlock:4.4.0@aar'

注意，一定要加@aar，否则有可能获取不到jar，而导致编译失败

关于@aar的描述，在[stackoverflow](https://stackoverflow.com/questions/26250790/what-does-aar-means-in-gradle-compile-task)上的描述如下：

        The AAR format is the binary distribution of an Android Library Project.
        As described here in the official Android Tools documentation.
        In your case, when adding a compile dependency in an Android Gradle project, adding "@aar" means that you would like to fetch the @aar file and not a regular JAR file.        
        
        