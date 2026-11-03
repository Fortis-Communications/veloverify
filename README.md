# VeloVerify for Claude, ChatGPT and Codex

> **Not available yet.** The VeloVerify connection opens when it is announced on [verifyapi.veloconnect.me](https://verifyapi.veloconnect.me). Until then, connecting will fail.

Check phone numbers from your VeloVerify account inside Claude, ChatGPT and Codex. See whether a number is live, which network serves it and whether it was ported, for one number or a list of up to 1000. You can also see your balance, usage and prices.

## Connect

You need a VeloVerify account and an API key. Create a key under **API Keys** in your portal. A key with an IP restriction can't connect, so create a separate key for this.

When you connect, a VeloVerify sign-in page opens. Enter your API key and secret there, never in a chat. Tick **allow paid lookups** only if you want the assistant to be able to run them.

## Tools

| Tool | What it does | Charges your balance |
|---|---|---|
| `get_account_balance` | Shows your balance | No |
| `get_usage_summary` | Shows lookups and spend, by service | No |
| `list_recent_lookups` | Lists recent lookups, with numbers masked | No |
| `get_lookup_price` | Shows the price of a lookup | No |
| `list_destinations` | Lists countries and networks you can look up | No |
| `estimate_number_list` | Shows what a list would cost | No |
| `hlr_lookup` | Checks whether a number is live and its network | Yes |
| `mnp_lookup` | Finds a number's current network | Yes |
| `check_number_list` | Checks up to 1000 numbers | Yes |
| `get_list_results` | Shows a list's progress and results | No |

Paid tools are capped per day for each key. Your client asks you to confirm each paid call.

## Disconnect

Remove the connector in your AI app. To end every connection a key holds, rotate that key in your portal.

## Privacy

What you type, including phone numbers, is processed by your AI provider under its own terms, as well as by VeloVerify. See the [privacy policy](https://verifyapi.veloconnect.me/privacy). Only check numbers you have a legitimate reason to check.

## Support

<https://verifyapi.veloconnect.me/support>
