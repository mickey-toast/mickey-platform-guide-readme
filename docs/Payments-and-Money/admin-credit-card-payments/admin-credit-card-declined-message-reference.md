---
title: Card declined message reference
excerpt: >-
  When a card payment cannot be processed, the Toast POS device shows a message
  from the card network. These response messages can be difficult to interpret.
  The following table…
hidden: false
metadata:
  description: >-
    When a card payment cannot be processed, the Toast POS device shows a
    message from the card network. These response messages can be difficult to
    interpret. The following table…
---

When a card payment cannot be processed, the Toast POS device shows a message from the card network. These response messages can be difficult to interpret. The following table shows the response messages received most frequently on Toast POS devices with descriptions for why that message might appear.

> 📘 Note
>
> The messages and the descriptions shown in the following tables are produced by the card processor, not by Toast. The information provided in these tables is intended for reference only, and is subject to change without notice by the card network.

| Response Message | Descriptions |
|---|---|
| *REQUEST DENIED* | Do not honor |
| AUTH DECLINED | Do not honor<br>Transaction not permitted to issuer/cardholder<br>Exceeds withdrawal limit<br>Domain Restriction Controls Fail<br>Declined-transaction in violation of law<br>Declined PIN attempts |
| AUTH TRN NO AL'W | Auth transaction not allowed for this payment |
| CALL OPER | Refer to card issuer<br>Refer to call center |
| CALL VOICE OPER | Refer to card issuer<br>Re-enter transaction |
| CARD EXPIRED | Expiration date check failed<br>Expired card<br>Card expiry date less than current date |
| CARDHLDR DECLINE | Declined per cardholder request |
| CVD ERROR | Do not honor |
| DECLINED | Declined by user<br>Invalid effective date on card |
| ERR PROC FIELD | Format error, invalid value in message |
| HOLD - CALL | Pick up |
| INV CARD NUMBER | Invalid cardholder account<br>Account number not found in BIN table |
| INVALID AMOUNT | Invalid amount |
| INVALID CARD | Invalid card number |
| INVALID CARD NO | Invalid card number |
| INVALID EXP DATE | Invalid expiry date |
| INVALID FUNCTION | Transaction not permitted to terminal |
| INVALID MERC NO | Invalid merchant or terminal |
| INVALID PIN | Invalid pin |
| LOST/STOLEN CARD | Lost or stolen card |
| NO CHECKING ACCT | Error |
| PICK UP CARD | Pick up card<br>Decline - pick up card<br>Pick up card - No Fraud<br>Pick up card (Special Condition)<br>Pick up card (Special Condition)(Fraud Account)<br>Lost card - pick up<br>Stolen card - pick up |
| PIN TRIES EXCEED | Re-enter transaction |
| PROC ERROR 13 | System error |
| SECURITY VIOLATION | Security violation |
| TRAN NOT ALLOWED | Transaction not permitted to terminal |
| TRANS DENIED | Do not honor<br>Invalid cardholder account<br>Unable to locate record<br>Insufficient funds<br>Restricted card<br>Security violation<br>Account activity limit exceeded<br>Allowable number of PIN entry tries exceeded<br>One or more errors in message<br>File is unavailable<br>No credit account<br>Fraudulent activity detected |
| TRANS NOT ALLOW | Transactions not allowed to cardholder<br>Transactions not allowed to terminal<br>Illegal transaction - violation of law<br>Capture transactions not allowed for this payment type<br>Capture transaction on authorization only terminal<br>Private label transaction not allowed for terminal<br>Store reporting transactions not allowed |
