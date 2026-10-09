```
fiber-pay peer list --json
{
  "success": true,
  "data": {
    "peers": [
      {
        "pubkey": "026a4a82e31887b9223b49a45715c30f6cc796838fa61c832b7a587fc15b83973e",
        "address": "/ip4/157.230.84.72/tcp/9227/p2p/QmPNCwpTUkDVVeu4VpjV7XJPZBPswj1Y7cc3h9cmneyY1r"
      },
      {
        "pubkey": "0262dafc075994862492d66752591dc790210e32a298bd934339298fcf10d00f61",
        "address": "/ip4/16.162.99.28/tcp/8230/p2p/QmfNUEDq9ZqH8oC55hANNS1CwenCn6ht1as3PufZU1kGjR"
      },
      {
        "pubkey": "03698c4b37049adb4f28a3eb2aa2a57f0a56cf25959a4d2161df5597f23c7d7d94",
        "address": "/ip4/157.230.15.176/tcp/8228/p2p/QmbsNpwt8zpXoTMFg1xDUq5qpNvcdZQfeykbKMY9nd8e1H"
      },
      {
        "pubkey": "030316914a75e8f18faf82e8e6dd166f2aaa1f96105f98c099be4f3be073140eaf",
        "address": "/ip4/3.212.70.79/tcp/18228/p2p/QmQC7fV1ji7aoAyjsHNwdYLLxXseikPH1Auo7ChsvRVFtq"
      }
    ]
  }
}
```

```
fiber-pay channel open --peer "/ip4/54.179.226.154/tcp/8228/p2p/Qmes1EBD4yNo9Ywkfe6eRw9tG1nVNGLDmMud1xJMsoYFKy" --funding 200 --json
{
  "success": true,
  "data": {
    "temporaryChannelId": "0x9a04ef71d2cb5070f91dc80ed66914cd532c529c817f9ef0eb5c14bd81c57109",
    "peer": "0x024714ca19abea4ddc0f3863ffdfb2e2cee76af87c477de4bc67c74a83f8140042",
    "fundingAmount": "20000000000",
    "fundingLabel": "CKB"
  }
}
```

```
fiber-pay channel watch --until CHANNEL_READY --json
{"event":"snapshot","ts":"2026-10-09T12:55:15.385Z","data":{"channels":[{"channelId":"0x9a9b816c567508e0bfe1b539d44ef745cf5636b55d56459f8457cbf08da9281d","channelIdShort":"0x9a9b816c...8da9281d","pubkey":"024714ca19abea4ddc0f3863ffdfb2e2cee76af87c477de4bc67c74a83f8140042","pubkeyShort":"024714ca19...f8140042","state":"CHANNEL_READY","stateLabel":"✅ Channel Ready","localBalance":101,"remoteBalance":0,"capacity":101,"localBalanceCkb":101,"remoteBalanceCkb":0,"capacityCkb":101,"unit":"CKB","balanceRatio":"100/0","pendingTlcs":0,"enabled":true,"isPublic":true,"age":"1m ago"}],"summary":{"count":1,"activeCount":1,"totalLocalCkb":101,"totalRemoteCkb":0,"totalCapacityCkb":101,"udtTotals":[]}}}
{"event":"terminal","ts":"2026-10-09T12:55:15.386Z","data":{"reason":"target_state_reached","untilState":"CHANNEL_READY"}}
```

```
fiber-pay channel list --json
{
  "success": true,
  "data": {
    "channels": [
      {
        "channel_id": "0x9a9b816c567508e0bfe1b539d44ef745cf5636b55d56459f8457cbf08da9281d",
        "is_public": true,
        "is_acceptor": false,
        "is_one_way": false,
        "channel_outpoint": "0x68976162543c870ea8ebb8ba48044797f00ceffabde98f55613700a9d2f87dbc00000000",
        "pubkey": "024714ca19abea4ddc0f3863ffdfb2e2cee76af87c477de4bc67c74a83f8140042",
        "funding_udt_type_script": null,
        "state": {
          "state_name": "CHANNEL_READY"
        },
        "local_balance": "0x25a01c500",
        "offered_tlc_balance": "0x0",
        "remote_balance": "0x0",
        "received_tlc_balance": "0x0",
        "pending_tlcs": [],
        "latest_commitment_transaction_hash": "0x7ab7ea2a042273a1aa067754c6ba76e295523d1c784334ccafa390638d720f02",
        "created_at": "0x1a120ba19c2",
        "enabled": true,
        "tlc_expiry_delta": "0xdbba00",
        "tlc_fee_proportional_millionths": "0x3e8",
        "shutdown_transaction_hash": null,
        "failure_detail": null
      }
    ],
    "count": 1
  }
}
```
