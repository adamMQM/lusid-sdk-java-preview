

# Future

LUSID representation of a Future.  Including, but not limited to, Equity Futures, Bond Futures, Index Futures, Currency Futures, and Interest Rate Futures.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**startDate** | **OffsetDateTime** | The start date of the instrument. This is normally synonymous with the trade-date. | 
**maturityDate** | **OffsetDateTime** | The final maturity date of the instrument. This means the last date on which the instruments makes a payment of any amount.  For the avoidance of doubt, that is not necessarily prior to its last sensitivity date for the purposes of risk; e.g. instruments such as  Constant Maturity Swaps (CMS) often have sensitivities to rates that may well be observed or set prior to the maturity date, but refer to a termination date beyond it. | 
**identifiers** | **Map&lt;String, String&gt;** | External market codes and identifiers for the bond, e.g. ISIN. | 
**contractDetails** | [**FuturesContractDetails**](FuturesContractDetails.md) |  | 
**contracts** | **java.math.BigDecimal** | The number of contracts held. |  [optional]
**refSpotPrice** | **java.math.BigDecimal** | The reference spot price for the future at which the contract was entered into. |  [optional]
**underlying** | [**LusidInstrument**](LusidInstrument.md) |  |  [optional]
**calculationType** | **String** | Calculation type for some Future instruments which have non-standard methodology.  Optional, if not set defaults as follows:  - If ExchangeCode is \&quot;ASX\&quot; and ContractCode is \&quot;IR\&quot; or \&quot;BB\&quot; set to ASX_BankBills  - If ExchangeCode is \&quot;ASX\&quot; and ContractCode is \&quot;YT\&quot; set to ASX_3Year  - If ExchangeCode is \&quot;ASX\&quot; and ContractCode is \&quot;VT\&quot; set to ASX_5Year  - If ExchangeCode is \&quot;ASX\&quot; and ContractCode is \&quot;XT\&quot; set to ASX_10Year  - If ExchangeCode is \&quot;ASX\&quot; and ContractCode is \&quot;LT\&quot; set to ASX_20Year  - otherwise set to Standard    Specific calculation types for ASX bond futures are:  - [Standard] The default calculation type, which does not fit into any of the categories below.  - [ASX_BankBills] Used for AUD and NZD futures “IR” and “BB” on ASX. 90D Bank Bills.  - [ASX_3Year] Used for “YT” on ASX. 3YR semi-annual bond (6 coupons) @ 6%.  - [ASX_5Year] Used for “VT” on ASX. 5yr semi-annual bond (10 coupons) @ 2%.  - [ASX_10Year] Used for “XT” on ASX. 10yr semi-annual bond (20 coupons) @ 6%.  - [ASX_20Year] Used for “LT” on ASX. 20yr semi-annual bond (40 coupons) @ 4%.    Supported string (enumeration) values are: [Standard, ASX_BankBills, ASX_3Year, ASX_5Year, ASX_10Year, ASX_20Year, B3_DI1]. |  [optional]



