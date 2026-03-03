# MCC Code Dataset — PointsPick

Free, open-source dataset of Merchant Category Codes (MCCs) and merchant-to-MCC mappings.

**Powered by [PointsPick](https://www.pointspick.com) — Credit Card Intelligence**

## What is an MCC Code?

A Merchant Category Code (MCC) is a 4-digit number assigned to businesses by payment networks
(Visa, Mastercard, Amex) to classify the type of business. Credit card rewards programs use
MCC codes to determine which bonus categories apply to purchases.

For example:
- MCC 5411 = Grocery Stores → grocery cards earn bonus
- MCC 5814 = Fast Food → dining cards earn bonus
- MCC 5300 = Wholesale/Warehouse → often earns NO grocery bonus

## Dataset Contents

| File | Description | Records |
|------|-------------|---------|
| `data/mcc_codes.csv` | All MCC codes with descriptions | 981 |
| `data/mcc_codes.json` | Same data in JSON format | 981 |
| `data/merchant_mappings.csv` | Merchant-to-MCC mappings | 6,569 |

## MCC Codes CSV Schema

```
code,description,category,is_bonus_eligible,visa_description
5411,Grocery Stores - Supermarkets,Grocery,true,GROCERY STORES
5814,Fast Food Restaurants,Dining,true,EATING PLACES/RESTAURANTS
...
```

## Merchant Mappings CSV Schema

```
merchant_name,slug,mcc_code,mcc_description,category
Amazon,amazon,5999,Misc. and Specialty Retail Stores,Retail
Starbucks,starbucks,5812,Eating Places - Restaurants,Dining
...
```

## Interactive Tools

- **MCC Lookup**: https://www.pointspick.com/tools/mcc-lookup
- **Best Card Finder**: https://www.pointspick.com/tools/card-finder
- **Embeddable Widget**: https://www.pointspick.com/widget/embed.html
- **Full API**: https://www.pointspick.com/api-docs.html

## License

MIT License — free to use with attribution.

If you use this dataset, please link to: https://www.pointspick.com/tools/mcc-lookup

## Last Updated

2026-03-03

## Attribution

Data sourced from ISO 18245 MCC standard, Visa/Mastercard published classifications,
and verified transaction processing records. Maintained by the PointsPick editorial team.
