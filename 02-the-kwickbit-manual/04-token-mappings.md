# Token-to-Currency Mapping Strategy Example

When integrating KwickBit with QuickBooks, an important step is deciding how to represent crypto transactions 
within the accounting software. Since QuickBooks does not natively support crypto currencies like XLM (Stellar Lumens)
or USDC (USD Coin), you have two main strategies for mapping these tokens: using a placeholder currency or
converting transactions directly into fiat currency.

## Token-to-Currency Mapping Strategy

### Placeholder Currency Mapping
You have the option to map each crypto token to a placeholder currency in QuickBooks. This approach is useful since QuickBooks does not support custom currencies. Select an exotic currency (one you will not use for other transactions) to represent your token in QuickBooks.

**Ideal** for tokens frequently used in transactions. It allows for detailed tracking within QuickBooks without affecting your primary financial reports in standard currencies.


### Direct Fiat Conversion
Alternatively, if you prefer not to use a placeholder currency, transactions can be directly converted to the fiat currency of the chosen accounts. This method is recommended for tokens with a minimal number of transactions, simplifying management in QuickBooks.

**Ideal** for tokens with fewer transactions. It simplifies the accounting process by converting crypto transactions into your primary fiat currency, reducing the need for managing multiple placeholder currencies.


**By thoughtfully selecting your mapping strategy, you can tailor KwickBit's QuickBooks integration to fit your accounting needs, ensuring accurate and efficient financial management across both crypto and traditional finance.**



### Example Using Placeholder Currency

Suppose you frequently transact with XLM and want to track these transactions in QuickBooks without converting them to fiat currency immediately. You could choose an exotic currency, such as the Belarusian Ruble (BYN), as a placeholder.

In this case, every XLM transaction in KwickBit would be represented in QuickBooks as a BYN transaction. This method allows you to maintain a clear record of XLM transactions without affecting your primary financial reports.

**Configuration Steps for XLM as a Placeholder:**
1. In the financial mappings modal, select an accounts receivable, an accounts payable, and a bank account, all set to use BYN as their currency.
2. Map the XLM token to BYN as the placeholder currency.
3. Ensure all XLM transactions are tracked under this setup to keep your accounting consistent.

### Example Using Direct Fiat Conversion

Alternatively, consider you use USDC for a limited number of transactions and prefer to convert these into your primary fiat currency to simplify your QuickBooks management.

If your primary fiat currency is USD, you can set KwickBit to automatically convert USDC transactions into USD based on the current exchange rate at the time of each transaction. This approach eliminates the need for a placeholder currency, streamlining the reconciliation process for tokens with fewer transactions.

**Configuration Steps for USDC Conversion to USD:**
1. Select your accounts receivable, accounts payable, and bank account in QuickBooks, ensuring they are denominated in USD.
2. Choose not to use a placeholder currency for USDC. Instead, opt for direct conversion to USD.
3. KwickBit will handle the conversion, allowing these transactions to be seamlessly integrated into your existing USD-denominated accounts.

**By carefully choosing your token-to-currency mapping strategy, you ensure that KwickBit's integration with QuickBooks accurately reflects your crypto transactions, aligning with your overall accounting practices and financial reporting needs.**
