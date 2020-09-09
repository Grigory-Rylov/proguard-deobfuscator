# De-obfuscator
## Usage:
```
DeObfuscator deObfuscator = new DeObfuscator(mappingFile);
// 1) get original class name
String originalClassName = deObfuscator.originalClassName(obfuscatedClassName);

// 2) get original method name
String originalMethodName = deObfuscator.originalMethodName(originalClassName, obfuscatedMethodName, type, argumetns)
```
where `type` and `arguments` can be null, but the result may be inaccurate


## Dependency
1. Add it in your root build.gradle at the end of repositories:
```
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
	}
}
```

2. Add the dependency
```
dependencies {
    implementation "com.github.Grigory-Rylov:proguard-deobfuscator:$version"
}
```
