
# Unterschreiben Sie den Mietvertrag!

Berlin used to be an affordable place not so long ago. When I moved to Berlin, my uncle was paying around 580 euros for a one-bedroom apartment in the Mitte neighborhood. From there, you could walk through history, art, and culture without even taking a bus. Things have changed since then. Berliners not only need to compete between thousands of applications to find a place, but also they need to pay hefty rents to secure what they want. 

I want to investigate this matter and answer some questions. More importantly, I decided to make a machine learning model predicting the rent prices in Berlin using different features. Since there are not many public datasets about berlin house prices available out there, I used a kaggle dataset. [This dataset](https://www.kaggle.com/corrieaar/apartment-rental-offers-in-germany) contains apartment rental offers in Germany from the dates 2018-09-22, 2019-05-10, and 2019-10-08 (Collected from [immobilienscout24](https://www.immobilienscout24.de)). I filtered out Berlin listings to work on it exclusively.

The berlin dataset is available on my Github.

* Gathered berlin listings from immobilienscout24, validated and cleaned data
* Performed an exploratory data analysis (plus AutoEDA) and answered different questions about the berlin real state market
* Built machine learning models to predict rent prices in berling using regression techniques
## Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `missingno`

AutoML by:
- `pandas_profiling`
- `AutoViz`

## Dataset

The variables of this dataset are:

- `regio1` - bundesland
- `serviceCharge` - aucilliary costs such as electricty or internet in €
- `heatingType` - type of heating
- `telekomTvOffer` - is payed TV included if so which offer
- `telekomHybridUploadSpeed` - how fast is the hybrid inter upload speed
- `newlyConst` - is the building newly constructed
- `balcony` - if a listing has a balcony
- `picturecount` - how many pictures were uploaded to the listing
- `pricetrend` - price trend as calculated by Immoscout
- `telekomUploadSpeed` - how fast is the internet upload speed
- `totalRent` - total rent (usually a sum of base rent, service charge and heating cost)
- `yearConstructed` - construction year
- `scoutId` - immoscout Id
- `noParkSpaces` - number of parking spaces
- `firingTypes` - main energy sources, separated by colon
- `hasKitchen` - has a kitchen
- `geo_bln` - bundesland (state), same as regio1
- `cellar` - has a cellar
- `yearConstructedRange` - binned construction year, 1 to 9
- `baseRent` - base rent without electricity and heating
- `houseNumber` - house number
- `livingSpace` - living space in sqm
- `geo_krs` - district, above ZIP code
- `condition` - condition of the flat
- `interiorQual` - interior quality
- `petsAllowed` - are pets allowed, can be yes, no or negotiable
- `street` - street name
- `streetPlain` - street name (plain, different formating)
- `lift` - is elevator available
- `baseRentRange` - binned base rent, 1 to 9
- `typeOfFlat` - type of flat
- `geo_plz` - ZIP code
- `noRooms` - number of rooms
- `thermalChar` - energy need in kWh/(m^2a), defines the energy efficiency class
- `floor` - which floor is the flat on
- `numberOfFloors` - number of floors in the building
- `noRoomsRange` - binned number of rooms, 1 to 5
- `garden` - has a garden
- `livingSpaceRange` - binned living space, 1 to 7
- `regio2` - District or Kreis, same as geo krs
- `regio3` - City/town
- `description` - free text description of the listing
- `facilities` - free text description about available facilities
- `heatingCosts` - monthly heating costs in €
- `energyEfficiencyClass` - energy efficiency class (based on binned thermalChar, deprecated since Feb 2020)
- `lastRefurbish` - year of last renovation
- `electricityBasePrice` - monthly base price for electricity in € (deprecated since Feb 2020)
- `electricityKwhPrice` - electricity price per kwh (deprecated since Feb 2020)
- `date` - time of scraping

![Berlin](berlin.jpeg)
