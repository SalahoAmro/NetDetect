# NetDetect
An Android library to check actual internet connectivity.

### How To Use

1. Add the JitPack repository to your build file. Add it in your root build.gradle at the end of repositories:
``` 
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
  ```
  
2. Add the dependency:
```
implementation 'com.github.SalahoAmro:NetDetect:Tag'
```

3. Initialize NetDetect in Application class:
```
NetDetect.init(this);
```

4. Use it anywhere!
```
NetDetect.check((isConnected -> Toast.makeText(this, isConnected + "", Toast.LENGTH_SHORT).show()));
```
