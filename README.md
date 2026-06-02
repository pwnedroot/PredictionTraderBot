 More Info: https://whop.com/cryptz-predictions-trader/cryptz-predictions-trader-75/

 

https://github.com/user-attachments/assets/58952c63-7854-4059-9609-64e177b75152


# Cryptz Trading Bot

## Preconfigured Virtual Machine for Polymarket Copy Trading

Cryptz Trading Bot is a ready-to-configure Linux virtual machine containing a Polymarket copy-trading bot, a local dashboard, setup scripts, and safety checks. It is designed for people who want a working foundation they can run, inspect, and customize without building an automation stack from scratch.

The product is delivered as a virtual machine. Import the VM into VMware, log into your own Bullpen account, run the guided setup script, choose your risk limits, and test the bot in dry-run mode before deciding whether to enable live trading.

## What the Bot Does

The bot monitors selected Polymarket trader wallets and looks for new trades. When a watched trader places a trade, the bot evaluates the signal against your local settings before taking any action.

For a buy to be copied, it must pass configurable checks such as:

- Trade freshness, so old activity is not copied after the bot restarts.
- Available bankroll and daily spending limits.
- Maximum amount per copied trade.
- Maximum number and total cost of open positions.
- Market status, trading availability, volume, spread, and liquidity.
- Entry-price protection, so the bot does not blindly chase a worse price.
- Cooldowns and other small-bankroll safeguards.

When live mode is enabled, approved trades can be placed automatically through the Bullpen CLI. The bot can also mirror sells for positions it previously copied and can use configured take-profit and stop-loss rules.

## How It Works

1. The bot watches a configured list of trader wallets and can refresh its watchlist using leaderboard filters when that feature is enabled.
2. It polls for new wallet activity at a configurable interval.
3. It ignores stale trades and screens each new buy against your risk and market-quality settings.
4. It sizes eligible copies proportionally, then applies your hard caps.
5. In dry-run mode, it records what it would do without placing orders.
6. In live mode, it submits approved Polymarket orders through your authenticated Bullpen account.
7. It keeps local logs and tracked-position state so you can review recent activity.

The bot is selective by design. Seeing a watched wallet trade does not mean the bot will copy it. A signal may be skipped because of price movement, insufficient liquidity, spending limits, existing exposure, stale timing, or another configured guardrail.

## What You Receive

- A preconfigured Linux virtual machine.
- The Cryptz copy-trading bot and editable configuration.
- A guided setup script that installs dependencies and verifies readiness.
- A safe dry-run mode for testing without placing trades.
- A local browser dashboard for starting, stopping, and monitoring the bot.
- A terminal interface and local event logs for deeper visibility.
- A diagnostic script for checking dependencies and Bullpen authentication.
- Setup documentation for importing and running the VM.

The VM is intended to shorten setup time. You still log into your own accounts, choose your own limits, and decide whether to use live trading.

## What This Product Is Not

Cryptz Trading Bot is not:

- A guaranteed-profit system.
- Financial advice or a recommendation to trade any market.
- A managed investment service.
- A custody service. You use your own Bullpen account and remain responsible for it.
- A promise that every watched-wallet trade will be copied.
- A fully finished consumer application with every edge case automated.
- A replacement for testing, monitoring, and making your own risk decisions.

Prediction markets are risky. Copied traders can lose money. Prices can move before your order reaches the market. Liquidity can be limited. Software and third-party services can fail. Only use funds you can afford to lose.
