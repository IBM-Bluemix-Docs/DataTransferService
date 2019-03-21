---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:new_window: target="_blank"}

# データ転送サービスの概説
{: #gettingstarted}

お客様は {{site.data.keyword.BluSoftlayer_full}} データ転送サービスを利用して、{{site.data.keyword.BluSoftlayer}} データ・センターに USB 2.0 または USB 3.0 互換のデバイス、CD、および DVD を送信できます。 お客様のデバイスはお客様のネットワークに直接接続されているので、リモートからデータ転送を制御できます。 デバイスは、カスタマー・データ・センター内の専用ラックに格納され、iSCSI ターゲットとしてマウントされます。 このデータ転送サービスは、{{site.data.keyword.BluSoftlayer}} のプライベート・ネットワークを使用せずに大量のデータを転送する必要がある場合に最適です。このサービスは {{site.data.keyword.BluSoftlayer}} のすべてのお客様に無料で提供されます。

## データ転送サービス画面にアクセスする

**注**: この画面は、アカウントのマスター・ユーザーのみが利用できます。

1. 固有の資格情報を使用して、[{{site.data.keyword.slportal}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){:new_window} にアクセスします。
2. ナビゲーション・バーから**「ストレージ」**>**「データ・マイグレーション」**>**「データ転送」**を選択して、データ転送サービス画面にアクセスします。 <br/>

**「データ転送サービス」**画面で、ユーザーはデータ転送要求の送信、要求に関する詳細の表示、デバイス追跡に関連したチケット履歴の表示、および既存の要求のキャンセルを行うことができます。

## データ転送要求を送信する

データ転送要求は、弊社データ・センターの担当者にお客様からの送付予定を知らせるように設計されています。 要求は [{{site.data.keyword.slportal}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){:new_window} 経由で送信されます。

要求を作成する際、以下のガイドラインを念頭に置いてください。

- 送付するデバイスがすべての[ハードウェア要件](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html)を満たしていることを確認してください。
- 要求 1 件に関連付けられるデバイスは 1 つだけです。 複数のデバイスを送る場合は、デバイスごとに新規要求を作成する必要があります。
- デバイスの返却が必要な場合は、転送期間の終了後にデバイスを返却できるように、送料支払い済みの返送用ラベルと輸出書類を必要に応じて同梱してください。
- 国際配送の場合、デバイスに関するすべてのライセンスの取得、配送、通関手続きをお客様が行う必要があります。 これには、関税、税金、{{site.data.keyword.BluSoftlayer}} データ・センターへの配送料、データ・センターからの配送料 (該当する場合) の支払いが含まれます。
- 要求を入力するときに、データ・センターへの配送を行う配送業者名と追跡番号を指定する必要があります。  データ転送要求を送信する前に、適切なデータ・センターの住所を指定した送付用ラベルを作成してください。

以下のステップに従ってデータ転送要求を送信します。

1. [{{site.data.keyword.slportal}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){:new_window} の**「データ転送サービス」**画面にアクセスします。
2. **「データ転送要求の注文 (Order Data Transfer Request)」**をクリックします。
3. 表 1 に従って、**「デバイス情報」**セクションの各フィールドに入力します。
<table border="1">
<caption>表 1 の左側は要求フォームのフィールド名、右側はその説明です。</caption>
 <tr><th>フィールド名</th><th>説明</th></tr>
 <tr><td>デバイス・タイプ</td><td>宛先に送られるデバイスのタイプ。 デバイス・タイプがリストされていない場合は、「その他」を選択します。</td></tr>
 <tr><td>シリアル番号</td><td> デバイスのシリアル番号。</td></tr><tr><td>説明</td><td>デバイスの簡単な説明。 入力すべき重要な情報としては、色、ラベル、ステッカーといった識別要素などがあります。</td></tr>
 <tr><td>注記</td><td>デバイスまたは転送に関するその他の注意事項。</td></tr><tr><td>宛先</td><td>デバイスを受け取るデータ・センター。</td></tr>
 <tr><td>配送業者</td><td>デバイスを宛先に配送するために使用する郵便業者または配送業者。</td></tr>
 <tr><td>追跡番号</td><td>発送の完全な追跡番号。</td></tr>
 </table>

4. **「返却用アドレス」**セクションの各フィールドに入力するか、**「会社アドレス」**チェック・ボックスを選択して、登録されている会社の住所がフィールドに自動的に取り込まれるようにします。 <br/> **注**: 送料支払い済みの返送用ラベルと必要な輸出書類を忘れずに同梱してください。
5. サービス契約を読んでから、**「データ転送サービス契約とマスター・サービス契約を読み、同意します」**チェック・ボックスを選択します。
6. **「サービス要求の送信」**をクリックします。

要求を送信した後、要求チケットの状況は`「SoftLayer に送信済み (Sent to SoftLayer)」`と表示されます。 地元の自治体からのライセンスが必要な輸出入については、その旨を {{site.data.keyword.BluSoftlayer}} に通知し、チケットにライセンス情報を添付してください。

デバイスを受け取ると、状況が`「SoftLayer で受領」`に更新されます。 データ・センターの技術員がデバイスをネットワークに接続すると、チケットの状況が再び更新されて`「接続済み」`になります。

初期データ転送期間は 2 週間です。 この期間中、デバイスへのアクセスはアカウントの管理者にのみ付与されます。 必要に応じて延長を要求できます。 また、2 週間を待たずにデバイスを返却してもらいたい場合は、返却を要求できます。 転送が完了したら、[{{site.data.keyword.slportal}}](https://control.softlayer.com/)で {{site.data.keyword.IBM}} に通知する必要があります。 その後、{{site.data.keyword.BluSoftlayer}} がデバイスを取り外し、お客様の要求に応じて返却または破棄します。


## 配送物画面にアクセスする

[{{site.data.keyword.slportal}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){:new_window} 内の配送物画面には、データ転送サービスの要求に関連付けられたすべての配送物が表示されます。この画面から配送物を確認し、返却された品を受領時に確認することができます。

配送物画面にアクセスするには、次のようにします。

1. 固有の資格情報を使用して、[{{site.data.keyword.slportal}} ![外部リンク・アイコン](../../icons/launch-glyph.svg "外部リンク・アイコン")](https://control.softlayer.com/){:new_window} にアクセスします。
2. ナビゲーション・バーから**「アカウント」**>**「管理」**>**「配送物 (Shipments)」**を選択します。

配送物画面では、過去 30 日に行われたすべての配送要求の詳細が表示されます。 状況、経過時間、または配送物の特定の詳細情報を基準にして、配送物を[ソートまたはフィルタリング](sort-or-filter-shipments-list.html)できます。 さらにこの画面で返却された品の受領確認を行うこともできます。![配送物画面](/images/DTSShipmentScreen1.png)