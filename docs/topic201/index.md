# Linuxカーネル

## 201.1 カーネルコンポーネント

| 重要度   | 説明 |
| :------: | ---- |
|        2 | 特定のハードウェア、ハードウェアドライバ、システムリソース、要件に必要なカーネルコンポーネントを利用できるようになること。この目標には、さまざまなタイプのカーネルイメージの実装、安定した長期的なカーネルとパッチの理解、およびカーネルモジュールの使用が含まれます。|

### 重要な項目

- カーネル2.6.x、3.x、4.xのドキュメント

??? "使用するファイル、用語、ユーティリティの一部のリスト"
    - /usr/src/linux/
    - /usr/src/linux/Documentation/
    - zImage
    - bzImage
    - xz compression

## 201.2 Linuxカーネルのコンパイル

| 重要度   | 説明 |
| :------: | ---- |
|        3 | 受験者は、必要に応じてLinuxカーネルの特定の機能を含めたり無効にしたりするために、カーネルを適切に設定することが期待されます。この目標には、必要に応じて Linux カーネルをコンパイルおよび再コンパイルすること、新しいカーネルを更新して変更点を指摘すること、initrd イメージを作成し、新しいカーネルをインストールすることが含まれます。|

### 重要な項目

- /usr/src/linux/
- kernel Makefile
- Kernel 2.6.x、3.x、4.x の make ターゲット
- 現在のカーネル設定をカスタマイズする。
- 新しいカーネルと適切なカーネルモジュールを構築する。
- 新しいカーネルと任意のモジュールをインストールする。
- ブートマネージャが新しいカーネルと関連ファイルを見つけられるようにする。
- モジュール設定ファイル
- DKMSを使用してカーネルモジュールをコンパイルする。
- dracutの理解

??? "使用するファイル、用語、ユーティリティの一部のリスト"
    - mkinitrd
    - mkinitramfs
    - make
    - make targets (all, config, xconfig, menuconfig, gconfig, oldconfig, mrproper, zImage, bzImage, modules, modules_install, rpm-pkg, binrpm-pkg, deb-pkg)
    - gzip
    - bzip2
    - module tools
    - /usr/src/linux/.config
    - /lib/modules/kernel-version/
    - depmod
    - dkms

## 201.3 カーネルランタイムの管理およびトラブルシューティング

| 重要度   | 説明 |
| :------: | ---- |
|        4 | 	2.6.x、3.x、4.xカーネルとそのロード可能なモジュールの管理および問い合わせができる。ブート時やランタイム時の一般的な問題を特定し、修正することができる。udev を使用したデバイスの検出と管理について理解している。この目的には、udev ルールのトラブルシューティングが含まれます。 |

### 重要な項目

- コマンドラインユーティリティを使用して、現在実行中のカーネルとカーネルモジュールに関する情報を取得する。
- カーネルモジュールを手動でロードおよびアンロードする。
- モジュールがいつアンロードされるかを決定する
- モジュールが受け取るパラメータを決定する
- モジュールをファイル名以外の名前でロードするようにシステムを設定する。
- /proc ファイルシステム
- /、/boot/、 および /lib/modules/ の内容
- 利用可能なハードウェアに関する情報を分析するツールやユーティリティ
- udevのルール

??? "使用するファイル、用語、ユーティリティの一部のリスト"
    - /lib/modules/kernel-version/modules.dep
    - module configuration files in /etc/
    - /proc/sys/kernel/
    - /sbin/depmod
    - /sbin/rmmod
    - /sbin/modinfo
    - /bin/dmesg
    - /sbin/lspci
    - /usr/bin/lsdev
    - /sbin/lsmod
    - /sbin/modprobe
    - /sbin/insmod
    - /bin/uname
    - /usr/bin/lsusb
    - /etc/sysctl.conf, /etc/sysctl.d/
    - /sbin/sysctl
    - udevmonitor
    - udevadm monitor
    - /etc/udev/
