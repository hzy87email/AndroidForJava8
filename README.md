# AndroidForJava8
##让Android Studio 支持java8语法

####步骤
 首先在app文件夹下面的build.gradle中添加如下代码:

<pre><code>
	apply plugin: 'me.tatarka.retrolambda'

	// 下面请添加在android大括号内
	
    compileOptions {
        sourceCompatibility JavaVersion.VERSION_1_8
        targetCompatibility JavaVersion.VERSION_1_8
    }

    retrolambda {
        javaVersion JavaVersion.VERSION_1_6
        javaVersion JavaVersion.VERSION_1_7
    }

</code></pre>


在module下面的build.gradle中添加如下代码

<pre><code>

    dependencies {
        classpath 'me.tatarka:gradle-retrolambda:3.2.1'
   }


</code></pre>



