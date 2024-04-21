---
sticker: ""
tag: oasis, module, blueprint
---
## Resources
1. Primary Power Storage Device
2. Load Balancer
3. Secondary Power Storage Device
4. Auxiliary Power Storage Devices
5. Micro-controller
6. Regulator
7. Transformer
8. Security Schema


```javascript

const data = [1,2,3,4,5,6,7,8,9]

data.forEach(i => (
console.log(`${i}-th: ${i ** i}`)
))
```



### Flowchart

```mermaid

graph TB

 LATENT_POWER["Latent Power"]
 ACTIVE_POWER["Active Power"]
 LOAD_BALANCER["Load  Balancer"]

 TRANSFORMER["Transformer"]

 UNIT["Unit"]

UNIT --> LATENT_POWER
UNIT --> ACTIVE_POWER

POWER["Power"]
```



## Constraints

### Blueprint

| New Column                  | Cost       | Link                                                                                                                                                                                                                                                                                                                                                                                                           | Status    | Types      | Priority | Quantity |
| --------------------------- | ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- | ---------- | -------- | -------- |
| Flooring Insulation         | -$128.00   | https://www.homedepot.com/p/Owens-Corning-FOAMULAR-150-1-in-x-4-ft-x-8-ft-R-5-Scored-Square-Edge-Rigid-Foam-Board-Insulation-Sheathing-20WE/207179253                                                                                                                                                                                                                                                          |           |            | 100      |          |
| Top Flooring                | -$124.00   | https://www.amazon.com/ProSource-fs-1908-pzzl-Puzzle-Exercise-Interlocking/dp/B00B4IHXRU/ref=sr_1_9?keywords=adhesive%2Bfoam%2Bworkout%2Bpad&sr=8-9&th=1                                                                                                                                                                                                                                                       |           |            | 100      |          |
| Wall and Ceiling Paneling   | -$180.00   | https://www.homedepot.com/p/Utility-Panel-Common-1-8-in-x-4-ft-x-8-ft-Actual-0-106-in-x-48-in-x-96-in-833096/100543684?source=shoppingads&locale=en-US&&mtc=SHOPPING-CM-CML-GGL-D21-021_001_PLYWOOD-NA-NA-NA-SMART-2996800-NA-NA-NA-NBR-NA-NA-NEW-Feed&cm_mmc=SHOPPING-CM-CML-GGL-D21-021_001_PLYWOOD-NA-NA-NA-SMART-2996800-NA-NA-NA-NBR-NA-NA-NEW-Feed-71700000107138821-58700008289641979-92700075338060853 |           |            | 100      | 9        |
| Wall and Ceiling Insulation |            |                                                                                                                                                                                                                                                                                                                                                                                                                |           |            | 100      |          |
| 800W Renogy Solar Panels    | -$675.00   | https://www.amazon.com/gp/product/B07JXYTFF7/ref=ox_sc_act_title_2?smid=A05654602L3XUQ70M87BV&psc=1                                                                                                                                                                                                                                                                                                            |           | power      | 100      | 8        |
| Inverter 2000W Pure Sine    | -$614.00   | https://www.amazon.com/gp/product/B07H9SXV61/ref=ox_sc_act_title_1?smid=ATVPDKIKX0DER&psc=1                                                                                                                                                                                                                                                                                                                    |           | power      | 100      | 2        |
| Foldable Bed Frame          | -$140.00   | https://www.amazon.com/AmazonBasics-Foldable-Platform-Under-Bed-Storage/dp/B073WRF565/ref=pd_rhf_d_cr_s_pd_crcbs_sccl_1_5/138-5899220-5956566?content-id=amzn1.sym.31346ea4-6dbc-4ac4-b4f3-cbf5f8cab4b9&pd_rd_i=B073WRLNS9&th=1                                                                                                                                                                                |           | Furniture  | 100      | 2        |
| Foldable Bed Mattress       | -$300.00   | https://www.amazon.com/MAXYOYO-Japanese-Mattress-Sleeping-Dormitory/dp/B0BF9JB5RW/ref=sr_1_9?keywords=futon+mattress+full+size&sr=8-9&ufe=app_do%3Aamzn1.fos.f5122f16-c3e8-4386-bf32-63e904010ad0                                                                                                                                                                                                              | #acquired | Furniture  | 100      | 2        |
| Fridge                      | -$360.00   | https://www.amazon.com/RFR322-B-Refrigerator-Freezer-Compartment-Adjustable-Control-Reversible-Apartment-Platinum/dp/B00IR8H55A/ref=sr_1_8?keywords=mini%2Bfridge&nav_sdd=aps&refinements=p_36%3A1253525011&rnid=386465011&s=home-garden&sr=1-8&ufe=app_do%3Aamzn1.fos.f5122f16-c3e8-4386-bf32-63e904010ad0&th=1                                                                                               |           | Appliance  | 100      |          |
| Surveillance Module         | -$60.00    | https://www.amazon.com/Mounting-Accident-Recording-Parking-Detection/dp/B0B7QX8GLC/ref=psdc_2230642011_t3_B098WVKF19                                                                                                                                                                                                                                                                                           |           | security   |          |          |
| Surveillance Module         | -$60.00    | https://www.amazon.com/Mounting-Accident-Recording-Parking-Detection/dp/B0B7QX8GLC/ref=psdc_2230642011_t3_B098WVKF19                                                                                                                                                                                                                                                                                           |           | security   |          |          |
| $1500 Savings               | -$1,500.00 |                                                                                                                                                                                                                                                                                                                                                                                                                | #reserved | allocation | 80       | 1        |
| Audio Speaker Set           | $30.00     |                                                                                                                                                                                                                                                                                                                                                                                                                |           |            |          |          |
| Parts Maintenance           | -$400.00   |                                                                                                                                                                                                                                                                                                                                                                                                                |           |            |          |          |
| Water Faucet                | -$50.00    |                                                                                                                                                                                                                                                                                                                                                                                                                |           | plumbing   | 100      | 2        |
| Sink 15x19x10               | -$420.00   | https://www.amazon.com/gp/product/B0849L4X96/ref=ox_sc_act_title_1?smid=A14VEZH60U86RN&psc=1                                                                                                                                                                                                                                                                                                                   |           | plumbing   | 100      | 2        |
| 6 Gal Water Storag          | -$102.00   | https://www.walmart.com/ip/Ozark-Trail-6-Gal-Water-Storage-Jug/16537207?wmlspartner=wlpa&selectedSellerId=0&wl13=5894&adid=2222222227716537207_117755028669_12420145346&wmlspartner=wmtlabs&wl0=&wl1=g&wl2=c&wl3=501107745824&wl4=pla-294505072980&wl5=9011796&wl6=&wl7=&wl8=&wl9=pla&wl10=8175035&wl11=local&wl12=16537207&wl13=5894&veh=sem_LIA                                                              |           | plumbing   | 100      | 6        |