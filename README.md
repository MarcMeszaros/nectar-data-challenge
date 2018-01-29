Nectar Data Challenge
=====================

You have 2 data sets - one data set is collected from the sensors (`used.csv`) and another one is collected from the point of sale system (`sold.csv`).

I would want you to correlate the 2 data sets using the following rules:
- you should match rows based on the `product_id` (this is the product that is being tracked by a given sensor or sold), time (this is the time when the products was used or sold) and `used_ml`/`sold_ml` (the amount that was used/sold) using the following rules:

- `product_id` should be matched 1:1 btw used and sold
- `time` should be within 20 minutes btw sold and used
- pick the closest `used_ml` vs `sold_ml` within the time window to get a 1:1 match

- There is some amount of nuance to the matching - don't worry too much about it, as long as it is an approximation of the rules.

There will be rows that won't match - you can simply ignore those.

Plot the distribution of the absolute difference between the `used_ml` and `sold_ml`, aggregated across all products and times.

Feel free to use any tools/programming languages you are most comfortable with. Also, feel free to ask for any clarifications you need.

Happy hacking!
