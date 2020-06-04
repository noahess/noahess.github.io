---
title: "Refined Electric Airplane & First-Order NPV Analysis"
date: 2020-06-04
categories:
- Aerospace
- Analysis
tags:
- Electrification
keywords:
- Boeing
- 767
- electric
- NPV
autoThumbnailImage: true
thumbnailImagePosition: "left"
thumbnailImage: images/electricNPV/thumbnail.jpg
coverImage: images/electricNPV/banner.jpg
metaAlignment: center
comments:       false
showActions:    false
---

A continuation of some previous work done analyzing an electrified 767-300.

<!--more-->

# Note

This analysis is still a work-in-progress

# Results

The value of an electrified airplane is highly dependent on both the price of electricity and a barrel of oil.
A correctly optimized airframe could provide incredible value for almost all stakeholders.

# Cost Comparison

The US Government has put together an incredible amount of data that has been highly valuable for this analysis.
Historic prices of a barrel of oil are from [the EIA](https://www.eia.gov/dnav/pet/hist/LeafHandler.ashx?n=PET&s=RWTC&f=M),
historical data for airline fuel costs are from [the BTS](https://www.transtats.bts.gov/fuel.asp?pn=1);
as well as detailed maintenance costs, amortization, fuel hours, etc from [Form 41, Schedule P-5.2](https://www.transtats.bts.gov/Fields.asp).

Comparing the historical price of a barrel of oil at WTI to the historical expense of one gallon of aviation fuel for Delta airlines, we get an average factor of 0.031507 for cost of a gallon of aviation fuel per cost of a barrel of oil, and a standard deviation of 0.0065049 from 1990-2019.

Looking at Form 41, Schedule P-5.2 for type 626 (767-300/ER), the average fuel consumption per hour is 1588.1 gallons with a standard deviation of 173.26 gallons.
The expected fuel consumption in gallons for three flight lengths is:

| 2 hours | 4 hours | 6 hours |
|---------|---------|---------|
| 3176.2  | 6352.5  | 9528.7  |

Using the nondimensional factor of cost per gallon = 0.031507 * price of barrel:

| WTI Spot Price | 2 Hr Fuel Cost | 4 Hr Fuel Cost | 6 Hr Fuel Cost |
|----------------|----------------|----------------|----------------|
|  $35           |  $3,503        |  $7,005        |  $10,508       |
|  $40           |  $4,003        |  $8,006        |  $12,009       |
|  $45           |  $4,503        |  $9,007        |  $13,510       |
|  $50           |  $5,004        |  $10,008       |  $15,011       |
|  $55           |  $5,504        |  $11,008       |  $16,512       |
|  $60           |  $6,005        |  $12,009       |  $18,014       |
|  $65           |  $6,505        |  $13,010       |  $19,515       |
|  $70           |  $7,005        |  $14,011       |  $21,016       |
|  $75           |  $7,506        |  $15,011       |  $22,517       |
|  $80           |  $8,006        |  $16,012       |  $24,018       |
|  $85           |  $8,506        |  $17,013       |  $25,519       |
|  $90           |  $9,007        |  $18,014       |  $27,020       |
|  $95           |  $9,507        |  $19,014       |  $28,521       |
|  $100          |  $10,008       |  $20,015       |  $30,023       |

Comparing to an electric airplane expectations:

| Electricity cost (/kWh) | 2 Hr (30 MWh) Electricity Cost | 4 Hr (60 MWh) Electricity Cost | 6 Hr (80 MWh) Electricity Cost |
|-------------------------|--------------------------------|--------------------------------|--------------------------------|
|  $0.06                  |  $1,800                        |  $3,600                        |  $4,800                        |
|  $0.07                  |  $2,100                        |  $4,200                        |  $5,600                        |
|  $0.08                  |  $2,400                        |  $4,800                        |  $6,400                        |
|  $0.09                  |  $2,700                        |  $5,400                        |  $7,200                        |
|  $0.10                  |  $3,000                        |  $6,000                        |  $8,000                        |
|  $0.11                  |  $3,300                        |  $6,600                        |  $8,800                        |
|  $0.12                  |  $3,600                        |  $7,200                        |  $9,600                        |
|  $0.13                  |  $3,900                        |  $7,800                        |  $10,400                       |
|  $0.14                  |  $4,200                        |  $8,400                        |  $11,200                       |
|  $0.15                  |  $4,500                        |  $9,000                        |  $12,000                       |
|  $0.16                  |  $4,800                        |  $9,600                        |  $12,800                       |
|  $0.17                  |  $5,100                        |  $10,200                       |  $13,600                       |
|  $0.18                  |  $5,400                        |  $10,800                       |  $14,400                       |

It's unlikely the average cost of a barrel of oil will be $40 or $100 over the next 20 years, and it's also unlikely electricity will only cost $0.06/kWh for airlines.

Assuming average future electricity costs to airlines are $0.10/kWh and a low/medium/high average gas prices of $55/$60/$65 / barrel at WTI; the savings per flight are:

| Scenario | 2 Hr Savings | 4 Hr Savings | 6 Hr Savings |
|----------|--------------|--------------|--------------|
| Low      |  $2,004      |  $4,008      |  $7,011      |
| Med      |  $2,504      |  $5,008      |  $8,512      |
| High     |  $3,005      |  $6,009      |  $10,014     |

Assuming there are 20 hours available to fly in a day, mandatory 1-hour turnaround times, and 320 days flying per year:

| Metric            | 2 Hr Missions | 4 Hr Missions | 6 Hr Missions |
|-------------------|---------------|---------------|---------------|
| Flights/day       | 6.67          | 4.00          | 2.86          |
| Days/yr           | 320           | 320           | 320           |
| Savings/yr Low    |  $5,342,155   |  $6,410,586   |  $7,782,770   |
| Savings/yr Medium |  $6,409,623   |  $7,691,548   |  $9,155,230   |
| Savings/yr High   |  $7,477,092   |  $8,972,510   |  $10,527,690  |


# Stay tuned!

