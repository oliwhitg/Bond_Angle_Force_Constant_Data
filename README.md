# Bond_Angle_Force_Constant_Data
Data and current code for analysing distributions of periodic systems.  Files will be updated as regularly as possible but will have the same names, so its worth redownloading the whole repo

## Results formatting
Results are split primarily by ringstats, and so the numbers in the results folders 

### ringstats_lt0.out
Ringstats are contained in this file

| MC Temperature | Bond force constr | Angle force contr | Seed number | pn (0-Max allowed ring size) |
| -------------- | ----------------- | ----------------- | ----------- | ---------------------------- |
| -1800 | 900 | 500 | 1 | 0.0                 0.0                 0.0                 0.0                 0.0                 0.0                 1.0                 0.0                 0.0 |     


### assortativities_lt0.out

| MC Temperature | Bond force constr | Angle force contr | Seed number | assortativity | estimated AW alpha | AW alpha | AW variance | AW r-squared | atomic assortativity |
| -------------- | ----------------- | ----------------- | ----------- | ------------- | ------------------ | -------- | ----------- | ------------ | --------------------------- |               
| -1800 | 1000 | 0 | 4 | -0.2102793 | 0.14734951 | 0.14749325 | 1.83782609 | 0.99902701 | nan |


### overall_mean_bond_length_ring.out
| MC Temperature | Bond force constr | Angle force contr | Seed number | Mean side length 5 membered | Mean side length 6 membered | Mean side length 7 membered |
| -1800 | 1000 | 0 | 3 | 1.0135110745400446 | 1.0173657880998375 | 1.0190479670215677 |

I'm not certain yet why they dont all average out to 0, I'm guessing some sort of energy contraint

### overall_mean_bond_length_ring.out

Mean ring edge, averaged across all rings of a given size in the system

| MC Temperature | Bond force constr | Angle force contr | Seed number | Mean side length 5 membered | Mean side length 6 membered | Mean side length 7 membered |
| -1800 | 1000 | 0 | 3 | 1.0135110745400446 | 1.0173657880998375 | 1.0190479670215677 |

I'm not certain yet why they dont all average out to 1, I'm guessing some sort of energy contraint

### ring_mean_bond_length_ring.out

Mean ring edge, averaged for each individual ring in the system
Each sample contains detail over two sequential lines


| MC Temperature | Bond force constr | Angle force contr | Seed number | List of ring sizes |
| -1800 | 900 | 500 | 1 | 6                   6                   6                   6                   6                   6                   6    ... |  
| MC Temperature | Bond force constr | Angle force contr | Seed number | List of mean edge length for each ring |
| -1800 | 900 | 500 | 1 | 0.9999997668749595  1.0000000555501014  1.0000000555501025  1.0000000555501014  1.0000000555501025  1.0000000555501014  0.9999997668749595  1.0000000555501014 ... |



