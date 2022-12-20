# ネットワーク構成

## 205.1 ネットワークの基本設定

| 重要度   | 説明 |
| :------: | ---- |
|        3 | 受験者は、ローカル、有線または無線、および広域ネットワークに接続できるようにネットワークデバイスを設定できることが期待されます。また、IPv4とIPv6の両方のネットワークを含む、1つのネットワーク内の様々なサブネット間で通信することができることも目標とします。 |

### 重要な項目

- イーサネットネットワークインターフェースの設定と操作のためのユーティリティ
- ワイヤレスネットワークへの基本的なアクセスを設定する

??? "使用するファイル、用語、ユーティリティの一部のリスト"
    - ip
    - ifconfig
    - route
    - arp
    - iw
    - iwconfig
    - iwlist

## 205.2 ネットワークの詳細設定

| 重要度   | 説明 |
| :------: | ---- |
|        4 | 受験者は、さまざまなネットワーク認証スキームを実装するためにネットワークデバイスを設定できることが期待されます。この目標には、マルチホームネットワークデバイスを設定し、通信問題を解決することも含まれます。 |

### 重要な項目

- ルーティングテーブルを操作するためのユーティリティ
- イーサネットネットワークインターフェースの設定と操作のためのユーティリティ
- ネットワークデバイスの状態を解析するユーティリティ
- TCP/IP トラフィックの監視と解析のためのユーティリティ

??? "使用するファイル、用語、ユーティリティの一部のリスト"
    - ip
    - ifconfig
    - route
    - arp
    - ss
    - netstat
    - lsof
    - ping, ping6
    - nc
    - tcpdump
    - nmap

## 205.3 ネットワークに関するトラブルシューティング

| 重要度   | 説明 |
| :------: | ---- |
|        4 | 基本的な設定ファイルやコマンドの場所を含め、一般的なネットワーク設定の問題を特定し、修正することができること。 |

### 重要な項目

- アクセス制限ファイルの場所と内容
- イーサネットネットワークインターフェースの設定と操作のためのユーティリティ
- ルーティングテーブルを管理するためのユーティリティ
- ネットワークの状態を一覧表示するユーティリティ
- ネットワーク構成に関する情報を得るためのユーティリティ
- 認識されているハードウェアデバイスと使用されているハードウェアデバイスに関する情報を得るための方法
- システム初期化ファイルとその内容 (Systemd と SysV init)
- NetworkManager の認識とネットワーク構成への影響

??? "使用するファイル、用語、ユーティリティの一部のリスト"
    - ip
    - ifconfig
    - route
    - ss
    - netstat
    - /etc/network/, /etc/sysconfig/network-scripts/
    - ping, ping6
    - traceroute, traceroute6
    - mtr
    - hostname
    - System log files such as /var/log/syslog, /var/log/messages and the systemd journal
    - dmesg
    - /etc/resolv.conf
    - /etc/hosts
    - /etc/hostname, /etc/HOSTNAME
    - /etc/hosts.allow, /etc/hosts.deny