# 5.1 1対1のコミュニケーション

サーバとサーバのトラフィックのほとんどは、サーバ同士が会話しているわけではないので、1対1の通信は通常クライアントによって行われます。クライアントが互いに会話する手段を提供するために、すべてのサーバは、任意のクライアントに到達するために、スパニングツリーに沿って正確に1方向にメッセージを送信できることが必要です。したがって、メッセージが配送される経路は、スパニングツリー上の任意の2点間の最短経路となります。

```
    1--\
        A        D---4
    2--/ \      /
          B----C
         /      \
        3        E

 Servers: A, B, C, D, E Clients: 1, 2, 3, 4

 [ 図1. 小規模 IRC ネットワークの例 ]
```

以下の例は、すべて上記の図1を参照しています。

例1：クライアント 1 と 2 間のメッセージは、サーバ A だけが見ることができ、サーバー A はそれをそのままクライアント 2 に送ります。

例2：クライアント 1 とクライアント 3 間のメッセージは、サーバ A と B、およびクライアント 3 が見ることができます。他のクライアントやサーバはそのメッセージを見ることができません。

例3：クライアント 2 と 4 間のメッセージは、サーバ A、B、C、D とクライアント 4 のみによって見られます。