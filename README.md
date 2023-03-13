# Tonkeeper Wallet

> 已经下载并安装在手机。依赖包已下载，还未编译成`android.apk`。

[![License](https://img.shields.io/github/license/tonkeeper/wallet)](LICENSE)
[![Release](https://img.shields.io/github/v/release/tonkeeper/wallet)](https://github.com/tonkeeper/wallet/releases)

**[tonkeeper.com](https://tonkeeper.com)**


Welcome to Tonkeeper repository.
If you have questions or suggestions, please file an [Issue](https://github.com/tonkeeper/wallet/issues/new/choose).

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

## License

The code and data files in this distribution are licensed under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
See https://www.gnu.org/licenses/ for a copy of this license.

See [LICENSE](LICENSE) file.


This project is tested with [Browserstack](https://browserstack.com).