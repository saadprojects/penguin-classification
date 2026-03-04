# Data Folder

## Dataset Information

This project uses the **Palmer Archipelago Penguins** dataset.

### Download Instructions

1. **Option 1: Direct Download**
   - Visit: https://github.com/allisonhorst/palmerpenguins
   - Download `penguins_size.csv`
   - Place it in this `data/` folder

2. **Option 2: Using Python**
   ```python
   import pandas as pd
   
   # Load directly from URL
   url = "https://raw.githubusercontent.com/allisonhorst/palmerpenguins/main/inst/extdata/penguins.csv"
   df = pd.read_csv(url)
   
   # Save locally
   df.to_csv('data/penguins_size.csv', index=False)
   ```

3. **Option 3: Using seaborn**
   ```python
   import seaborn as sns
   
   # Load the built-in dataset
   df = sns.load_dataset('penguins')
   
   # Save locally
   df.to_csv('data/penguins_size.csv', index=False)
   ```

### Dataset Description

- **Samples**: 344 penguins
- **Species**: Adelie, Chinstrap, Gentoo
- **Measurements**: 
  - Culmen length (mm)
  - Culmen depth (mm)
  - Flipper length (mm)
  - Body mass (g)
- **Location**: Palmer Archipelago, Antarctica
- **Years**: 2007-2009

### Citation

If you use this dataset, please cite:

```
Horst AM, Hill AP, Gorman KB (2020). palmerpenguins: Palmer Archipelago (Antarctica) 
penguin data. R package version 0.1.0. 
https://allisonhorst.github.io/palmerpenguins/
```

### Note

The `.csv` file is not included in this repository to keep the repo size small. 
Please download it using one of the methods above.
