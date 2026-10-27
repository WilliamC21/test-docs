# Create a Market

A **market** is a trading pair, such as `BTC/USDT`.

## Steps

1. Open **Dashboard → Markets**.
2. Click **Add market**.
3. Pick the base and quote assets.
4. Click **Save**.

{% tabs %}
{% tab title="Dashboard" %}
Use the steps above — no code needed.
{% endtab %}

{% tab title="API" %}
```bash
curl -X POST https://api.example.com/v2/markets \
  -H "Authorization: Bearer YOUR_KEY" \
  -d '{"base":"btc","quote":"usdt"}'
```
{% endtab %}
{% endtabs %}

{% hint style="warning" %}
A market can't be deleted while it has open orders.
{% endhint %}
