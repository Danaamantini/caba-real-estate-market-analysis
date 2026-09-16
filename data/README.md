# Data

## Dataset Source

**Property Listings for 5 South American Countries**  
Source: Properati Data, distributed through Kaggle by Rasmus Jacobsen.

[Download the dataset from Kaggle](https://www.kaggle.com/datasets/rmjacobsen/property-listings-for-5-south-american-countries)

This project uses the **Property Listings for 5 South American Countries** dataset, containing historical real estate listings from Properati.

## Source Files

The original dataset contains separate CSV files for:

- Argentina (`ar_properties.csv`)
- Colombia (`co_properties.csv`)
- Ecuador (`ec_properties.csv`)
- Peru (`pe_properties.csv`)
- Uruguay (`uy_properties.csv`)

This project uses the Argentina dataset and focuses on apartment listings that meet the following criteria:

- Location: Capital Federal (CABA)
- Property type: Apartment (`Departamento`)
- Operation type: Sale (`Venta`)
- Currency: USD

After filtering, the analytical population contains **121,442 listing records**.

## Data Files

The project uses three stages of processed data:

- `caba_apartments_base.csv` - filtered CABA apartment listings.
- `caba_apartments_clean.csv` - listings with valid price and surface information used for price-per-m2 analysis.
- `caba_apartments_final.csv` - final dataset containing engineered features used in the Tableau dashboard.

Raw and processed CSV files are intentionally excluded from this GitHub repository because of their size.

The transformation from raw data to the final analytical dataset is fully documented in the notebooks included in this repository.

## Important Notes

The dataset represents **property listings rather than confirmed transactions**. Prices are asking prices, and listing end dates should not be interpreted as confirmed sale dates.