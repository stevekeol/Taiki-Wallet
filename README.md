# Taiki Wallet

> 已经下载并安装在手机。依赖包已下载，还未编译成`android.apk`。

## Install dependencies

```bash
$ yarn install
```

##### For iOS run
```bash
$ yarn pods
$ yarn start:mobile
$ yarn run:ios
```

##### For Android run
```bash
$ yarn adb
$ yarn start:mobile
$ yarn run:android
```

More information about android build in [android readme](android/README.md).


## Adding icons

All icon files are named according to `ic-name-24.svg` scheme. And placed in `src/assets/icons/svg`.

After adding the icon, run the convert command

```bash
$ yarn icons
```

To convert you need `librsvg`.

If `librsvg` not already installed, run

```bash
$ brew install librsvg

# for ubuntu
$ sudo apt install librsvg2-bin
```

## 下载合适的jdk版本
1. [jdk-19](https://www.oracle.com/java/technologies/downloads/)
2. 移动到合适为位置：
	```shell title=""
	/usr/lib/jvm/jdk-19
	```
3. 配置 `./android/gradle.properties`
```
# Just for stevekeol
org.gradle.java.home=/usr/lib/jvm/jdk-19
```
