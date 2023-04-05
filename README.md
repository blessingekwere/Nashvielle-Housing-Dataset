# Nashvielle-Housing-Dataset
![](intro_pics11.jpg)
##### **Photo Source: Google**

## About Nashville
Nashville is the state capital of and most populous city in Tennessee and the seat of Davidson County. With a population of 689,447 at the 2020 U.S census. Nashville is the 21st most-populous city in the U.S, and the fourth most populous city in the southeastern U.S located on the Cumberland River the city is the center of the Nashville metropolitan area, which is one of the fastest growing in the nation.

![](Into_pics12.jpg)
##### **Photo Source: Google**

## About the Dataset: 
This dataset is about Nashville housing. The data contains 19 columns and 56,477 rows. The columns which are
* UniqueID  — Id number attributed to buyer
* ParcelID  — Code attributed to a land
* LandUse — Shows the different use of land
* SalesPrice — Cost of land
* LegalReference — Citation is the practice of crediting and referring to a authorized documents and sources.
* OwnerName: Name of land owner
* Acreage: The size of an area of land in acres
* LandValue: The worth of the land
* BuildingValue: Worth of the building
* YearBuilt: Year the building was built
* FullBath: A bathroom that includes shower, a bathtub, sink and toilet
* SaleDate: Date when the land was sold
* SaleAddress: Address of the land sold
* City: Location of the land
* OwnerAddress: Owner’s house address
* OwnerCity: City where the owner lives
* OwnerState: State where the owner lives

The link to the dataset can be found [here](https://medium.com/r/?url=https%3A%2F%2Fgithub.com%2Fblessingekwere%2FNashvielle-Housing-Dataset%2Fblob%2Fmain%2FNashville%2520Housing%2520Data%2520for%2520Data%2520Cleaning.xlsx)

## About the Project
This project is a data cleaning project of the Nashville Housing Dataset with the aim of ensuring that the data is fit to be used for further analysis after this.

## Tool Used
Microsoft SQL Server

## Observation in the data
There were few observation in the data which were
* Wrong formatting of date column
* Some rows in the property address had null values
* The property address column has both the city and house address in the same column
* The owner address has the state, city, and address in the same column
* Some rows in the SoldAsVacant has “Y” and “N” instead of “Yes” and “No”
* The data had some duplicate rows 
* The data had some columns that would not be needed for analysis

## Data Cleaning
The data was imported in a comma seperated value (csv) format into Microsoft SQL server using the import and export wizard and after that the data cleaning process commenced. Kindly follow through to see the steps I took to clean the data.

The first thing I had to do was to standardize the date format

![](Standardize%20Date%20format.png)

###### Standardizing date format in SaleDate column

I then proceeded to populate the property address column.

![](Populate%20Property%20Address%20Data.png)
###### Populating PropertyAddress column

After doing that I went on to break out the PropertyAddress column into Individual Columns

![](Breaking%20out%20Property%20Address%20into%20Individual%20Columns%20(Address%2C%20City%2C%20State).png)
###### Breaking out the PropertyAddress column into individual columns


 I also broke out the OwnerAddress column into Individual Columns
 
 ![](/Breaking%20out%20Owner%20Address%20into%20Individual%20Columns%20(Address%2C%20City%2C%20State).png)
 ###### Breaking out the OwnerAddress column into individual columns


I also updated the SoldAsVacant column with a “Yes” for “Y” and “No” for “N”

![](Updating%20SoldAsvacant%20from%20Y%20to%20Yes%20and%20N%20to%20No%20respectively.png)
###### Updating the SoldAsVacant column


Finally I decided to delete the unused columns or columns that will not be needed for further analysis of this project

![](Deleting%20unused%20columns.png)
###### Deleting Unused columns

## Conclusion
So far, I have been able to clean the data by transforming the data, formatting the columns correctly, removing columns that will not be useful for my analysis. 
Kindly drop your review. 

Your suggestions and recommendation will be highly appreciated.

Thank you :hugs:

