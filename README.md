# ormlite-sqlcipher
Patched OrmLite Android library with SQLCipher

# Installation

```sh
allprojects {  
    repositories {  
        jcenter()    
    }  
}
```

```sh
dependencies {  
    compile 'com.j256.ormlite.cipher:ormlite-sqlcipher:1.1@aar'
    compile 'com.j256.ormlite:ormlite-core:5.0'  
    compile 'com.j256.ormlite:ormlite-android:5.0'  
    compile 'net.zetetic:android-database-sqlcipher:3.5.3@aar'  
} 
```

# Usage

1. Init [sqlcipher](https://www.zetetic.net/sqlcipher/sqlcipher-for-android/).
2. Use in imports `com.j256.ormlite.cipher.android` imports instead of `com.j256.ormlite.android`
3. Use in imports `net.sqlcipher.database` imports instead of `android.database`
4. If you need `OrmLiteSqliteOpenHelper` override `getPassword` method

