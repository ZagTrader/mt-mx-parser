# ZagTrader MT/MX Parser

Free online parser for Swift MT and ISO 20022 (MX) messages: **[mt-mx-parser.zagtrader.com](https://mt-mx-parser.zagtrader.com/)**

Paste a message or open a message file and see the header blocks, every field with its name and decoded value, 16R/16S sequences, ISO 20022 element trees with element names and definitions, the key fields of each message family, and format checks for BIC, IBAN, ISIN, LEI, UETR, dates, amounts and mandatory fields. Parsing runs in your browser; nothing is uploaded. Format checks are not full network validation.

This repository holds documentation for the public tool. The tool itself is run by [ZagTrader](https://www.zagtrader.com/).

## What it reads

- **Input**: pasted text, or .txt, .fin, .out, .xml, .gz and .zip files.
- **Swift MT**: every category splits into fields, with names and checks for common types such as [MT103](https://mt-mx-parser.zagtrader.com/mt/mt103), [MT202](https://mt-mx-parser.zagtrader.com/mt/mt202), MT202COV, MT900, MT910, [MT940](https://mt-mx-parser.zagtrader.com/mt/mt940), MT942, MT950, [MT535](https://mt-mx-parser.zagtrader.com/mt/mt535) to MT537, [MT540](https://mt-mx-parser.zagtrader.com/mt/mt540) to [MT548](https://mt-mx-parser.zagtrader.com/mt/mt548) and [MT564](https://mt-mx-parser.zagtrader.com/mt/mt564) to MT568.
- **ISO 20022**: any message as an element tree, with key fields for [pacs.008](https://mt-mx-parser.zagtrader.com/mx/pacs.008), pacs.009, camt.052, [camt.053](https://mt-mx-parser.zagtrader.com/mx/camt.053), camt.054, camt.056, camt.029, [sese.023](https://mt-mx-parser.zagtrader.com/mx/sese.023), sese.024, sese.025, semt.002, semt.017 and the seev corporate action messages.

## Reference

| Page | Contents |
|---|---|
| [MT messages](https://mt-mx-parser.zagtrader.com/mt) | Swift MT message types by category, with fields and sequences |
| [MX messages](https://mt-mx-parser.zagtrader.com/mx) | ISO 20022 message families such as pacs, camt, sese, semt and seev |
| [Codes](https://mt-mx-parser.zagtrader.com/codes) | Qualifiers, indicators, [settlement status](https://mt-mx-parser.zagtrader.com/codes/settlement-status), [corporate action events](https://mt-mx-parser.zagtrader.com/codes/corporate-action-events) and [ISO 20022 external code sets](https://mt-mx-parser.zagtrader.com/codes/iso20022) |
| [Guides](https://mt-mx-parser.zagtrader.com/guides) | How MT and MX messages work, for example the [securities settlement lifecycle](https://mt-mx-parser.zagtrader.com/guides/securities-settlement-lifecycle) |
| [Troubleshooting](https://mt-mx-parser.zagtrader.com/troubleshooting) | Common message errors and what they mean |
| [Currencies](https://mt-mx-parser.zagtrader.com/currencies) | ISO 4217 currency codes with numbers, minor units and countries |
| [MIC codes](https://mt-mx-parser.zagtrader.com/mic) | ISO 10383 MICs of the exchanges ZagTrader connects to, with a link to the official list |
| [llms-full.txt](https://mt-mx-parser.zagtrader.com/llms-full.txt) | The MT and MX equivalence table and the example messages in plain text |

## Identifier checkers

Free checkers on the same site: [IBAN](https://mt-mx-parser.zagtrader.com/tools/iban-checker), [BIC](https://mt-mx-parser.zagtrader.com/tools/bic-checker), [UETR](https://mt-mx-parser.zagtrader.com/tools/uetr-checker), [ISIN](https://mt-mx-parser.zagtrader.com/tools/isin-checker), [CUSIP](https://mt-mx-parser.zagtrader.com/tools/cusip-checker), [SEDOL](https://mt-mx-parser.zagtrader.com/tools/sedol-checker), FIGI and CFI, and an [LEI search](https://mt-mx-parser.zagtrader.com/tools/lei-search). To find a security by ISIN, CUSIP, SEDOL, FIGI, ticker or name, use the [security lookup](https://www.zagtrader.com/tools/security-lookup) on zagtrader.com.

## MT and ISO 20022 equivalents

| Swift MT | ISO 20022 |
|---|---|
| MT103 | pacs.008 FI To FI Customer Credit Transfer |
| MT202 | pacs.009 Financial Institution Credit Transfer |
| MT202COV | pacs.009 Financial Institution Credit Transfer (cover) |
| MT101 | pain.001 Customer Credit Transfer Initiation |
| MT940, MT950 | camt.053 Bank To Customer Statement |
| MT942 | camt.052 Bank To Customer Account Report |
| MT900, MT910 | camt.054 Bank To Customer Debit Credit Notification |
| MT192, MT292 | camt.056 FI To FI Payment Cancellation Request |
| MT196, MT296 | camt.029 Resolution Of Investigation |
| MT540, MT541, MT542, MT543 | sese.023 Securities Settlement Transaction Instruction |
| MT544, MT545, MT546, MT547 | sese.025 Securities Settlement Transaction Confirmation |
| MT548 | sese.024 Securities Settlement Transaction Status Advice |
| MT535 | semt.002 Securities Balance Custody Report |
| MT536 | semt.017 Securities Transaction Posting Report |
| MT537 | semt.018 Securities Transaction Pending Report |
| MT564 | seev.031 Corporate Action Notification |
| MT565 | seev.033 Corporate Action Instruction |
| MT566 | seev.036 Corporate Action Movement Confirmation |
| MT567 | seev.034 Corporate Action Instruction Status Advice |
| MT568 | seev.038 Corporate Action Narrative |

The full table is on the [MX messages](https://mt-mx-parser.zagtrader.com/mx) page and in [llms-full.txt](https://mt-mx-parser.zagtrader.com/llms-full.txt).

## Related

- [ZagTrader FIX Parser](https://fixparser.zagtrader.com/) for FIX protocol messages and logs ([repository](https://github.com/ZagTrader/fix-parser))
- [Swift suite at ZagTrader](https://www.zagtrader.com/platform/swift-suite) and [settlement and post-trade](https://www.zagtrader.com/platform/settlement)
- [About the MT/MX Parser](https://mt-mx-parser.zagtrader.com/about): who builds it, where the content comes from and how to report a correction

© ZagTrader
