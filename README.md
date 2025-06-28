# US Plastic‑Surgery Cost & Surgeon‑Availability Dataset  
**Version:** v2507  **Last updated:** 2025‑07‑04

## What’s inside?
| Column | Description |
|--------|-------------|
| `City` | Metro / USPS‑state abbreviation |
| `Procedure` | Rhinoplasty, Breast Augmentation, Liposuction, Tummy Tuck, Facelift, Breast Reduction |
| `Avg_Cost_USD` | RealSelf average “Worth It Cost” (rounded to nearest \$50) |
| `Cost_Range_USD` | 25th–75th percentile range |
| `Board_Cert_Surgeons` | Count of individual NPIs with taxonomy 2082\* in metro |
| `Earliest_Consult_Days` | Days until next open slot via AestheticMatch API |
| `Financing?` | Yes/No flag (CareCredit / Alpheon accepted) |
| `Consult_Link` | Branded redirect → AestheticMatch booking form (affiliate) |

## Sources
* RealSelf Cost API – CC‑BY, accessed 2025‑07‑03  
* CMS NPPES monthly file 2025‑06 – public domain  
* AestheticMatch Availability Feed – used with permission  

## Refresh schedule
The GitHub Action `scheduler.yml` rebuilds the CSV every **Friday 02:00 UTC**  
and tags a new release `vYYMMDD`.  
Historical versions remain in `/data/`.

## Disclaimer
Prices are averages **for information only** and may change.  
Not medical advice.  Verify with a board‑certified plastic surgeon.  
Affiliate links are marked *Consult_Link*; I may receive a referral fee on booked consults.

**Raw CSV (70 kB)**  
https://raw.githubusercontent.com/Pastor0fMuppets/plastic-surgery-info/v2507/data/plastic_cost_v2507.csv

MIT License © 2025 FourGrowth
