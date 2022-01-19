```
Network Working Group                                           C. Kalt
Request for Comments: 2810                                   April 2000
Updates: 1459
Category: Informational
```


<h1 align="center">
Internet Relay Chat: アーキテクチャ
</h1>

## IRC

- [RFC 1459](https://solareenlo.com/rfc1459) (Internet Relay Chat Protocol)
- [RFC 2810](https://solareenlo.com/rfc2810) (Internet Relay Chat: Architecture)
- [RFC 2811](https://solareenlo.com/rfc2811) (Internet Relay Chat: Channel Management)
- [RFC 2812](https://solareenlo.com/rfc2812) (Internet Relay Chat: Client Protocol)
- [RFC 2813](https://solareenlo.com/rfc2813) (Internet Relay Chat: Server Protocol)
- [RFC 7194](https://solareenlo.com/rfc7194) (Default Port for Internet Relay Chat (IRC) via TLS/SSL)

## 本メモの位置づけ

このメモは、インターネットコミュニティーのための情報を提供するものです。このメモは、いかなる種類のインターネット標準も規定するものではありません。このメモの配布は無制限です。

## 著作権について

Copyright (C) The Internet Society (2000).  All Rights Reserved.

## 概要

IRC（Internet Relay Chat）プロトコルは、テキストベースの会議で使用するためのプロトコルです。1989年に BBS でユーザ同士がチャットをするために実装されて以来、発展してきました。

1993年5月に [RFC 1459 [IRC]](https://solareenlo.com/rfc1459) で初めて正式に文書化されたこのプロトコルは、進化を続けています。この文書は、現在の IRC プロトコルのアーキテクチャとその異なるコンポーネントの役割を説明する更新版です。他の文書では、ここで定義された様々なコンポーネント間で使用されるプロトコルを詳細に説明しています。
