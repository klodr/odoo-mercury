# odoo-mercury

Odoo 18 modules that connect Odoo to the public API of [Mercury](https://mercury.com).

> **Status:** code publication in progress. These modules already run in production on Odoo 18 and are being prepared for an open-source release in this repository.

## Modules

| Module | What it does | License |
|---|---|---|
| `payment_mercury` | **Pay with Mercury** payment provider. Each Odoo invoice creates a matching Mercury invoice; the customer pays by ACH or card on Mercury's hosted payment page, and a webhook records the payment and reconciles the invoice in Odoo. | LGPL-3 |
| `account_statement_import_online_mercury` | Online bank statement import from Mercury accounts (checking, savings and IO credit card), built on the OCA `account_statement_import_online` framework. | AGPL-3 |

Planned: payment of vendor bills from Odoo through Mercury's API, and handling of Mercury webhooks.

## Requirements

- Odoo 18.0
- A Mercury account and an API token, restricted to the IP address of the Odoo server

## Related project

- [mercury-invoicing-mcp](https://github.com/klodr/mercury-invoicing-mcp): MCP server for Mercury's banking and invoicing API.

## License

Each module declares its own license in its manifest (LGPL-3 or AGPL-3).

This project is not affiliated with or endorsed by Mercury Technologies, Inc.
