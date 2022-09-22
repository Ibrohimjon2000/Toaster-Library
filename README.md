# Toaster-Library
How to
To get a Git project into your build:

>Step 1. Add the JitPack repository to your build file

gradle
maven
sbt
leiningen
Add it in your root build.gradle at the end of repositories:
```
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```
>Step 2. Add the dependency
```
dependencies {
        implementation 'com.github.Ibrohimjon2000:Toaster-Library:0.1.0'
}
```
And now you can use the library in your activity
```
class MainActivity : AppCompatActivity() {
	override fun onCreate(savedInstanceState: Bundle?) {
                super.onCreate(savedInstanceState)
                setContentView(R.layout.activity_main)
                ToasterMessage().s(this,"Hello world")
       }
}
```
