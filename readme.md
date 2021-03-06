# _**Cargo Price Analysis**_

[Tableau Presentation](https://tabsoft.co/3RAjtq8)

## About This Project

Cargo price started to skyrocketed after the start of pandemic. The rising price of cargo make the activity of exporting to certain part of the world become extremely expensive. Riddled with this problem, I was asked to investigate the possible cause of this problem and project the possible time for the price to be back normal again.

## Objective

- Investigate the possible causes of the rising cargo price
- Project the possible date for normal cargo price

## Workflow

- Look for various economic dataset
- Make simple correlation and regression model in excel
- Import the strongest variables into input folder
- Do thorough analysis in python
- Make projection

## Discussion

After the initial investigation, I picked two variables as the main cargo price measurement:

- PPI (PCU483111483111)
- CASS
Using these two measurements, I also picked the following variables for each respective dependent variables:

## PPI

- 5-Year Breakeven Inflation Rate
- Household Spending Growth Expectation
- US Oil Price
- Retail Inventory to Sales Ratio
- Truck Transportation of Freight
- Retailers Sales

## CASS

- Los Angeles Port Loaded Import
- Autos: Inventories to Sales
- Household Spending Growth Expectation
- Retail Inventory to Sales Ratio
- Gold Price Expectation
- New Orders: Computer and Electronic Product

Each variables being used has certain connection with US consumer demand, inflation expectation, or input price. LA port loaded import is a good measures for how much imported goods being demanded by the US consumers, the higher the numbers mean higher port congestion that will happen. Retail inventory to sales ratio can also measure the ability of retailers to make appropriate inventory time to be sold, low ratio means the time it takes to sell an inventory is low, implying high demands from customers. Low inventory will force retailers to make more order of the requested goods, adding more pressure to the demand of cargo price assuming the goods come from outside of the country. New orders for computer and electronic product is also an important variable because, things like semiconductor chips come mostly from Taiwan, and being manufactured in China, therefore increasing demand for these things add more buying pressure for cargo price.

Another thing to address is people's inflation expectation. Measurement such as 5-year breakeven and household spending growth expectation gauge market expectation of the upcoming futures. Inflation can become some sort of self-fulfilling propehcy at a certain point. At higher inflation level, people are more likely to stocks up on goods, adding even more inflationary pressure they may have face already. Another inflation measures is the future gold price expectation. The future gold price expectation may gauge market feeling of future inflation uncertainty, thus making many people buying gold and having future rising price expectation of gold.

For US OIL price, this is an input price for many sectors. A higher oil price means higher end product price, assuming that the producer has pricing power over their product. Additionally, logistics activity requires oil to operate. Truck transportation of freight represent the price for trucking activity to the next logistic point or in reverse. This variables is a proxy for gauging the possible condition in the field, a higher price may indicate higher pricing power on the side of employee, despite the lower productivity of employee port in US coast, compared to their counterpart in China. This is important when gauging the export out of US.

I made some value assumption to the independent variables for the following 24 months. I primarily use numbers from the confidence interval, but for some extreme cases like auto inventory, i made some more liberal value assumption because the movement of auto inventory is extremely out of normal.

## Results

After making the underlying assumption, I used regression method to project the future value of the respective variables. By using the aforementioned methods, I predicted that at the earliest, the price may back to normal at mid 2024, 2 years from now.

## Credits

[Machine Learning Script Used](https://machinelearningmastery.com/)