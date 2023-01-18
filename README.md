# Kenya Counties, Constituencies, and Wards
This repository contains kenyan administrative units as a list of all the counties, constituencies, and wards  in the form of JSON objects in a single file called locations.txt. The data is organized hierarchically, with counties containing constituencies and constituencies containing wards.

## File Structure
locations.txt: A text file containing all the counties, constituencies, and wards in Kenya as JSON objects, where each JSON object has the following structure:
```

 counties = {
            "county_code": "county_name",
            ...
          }

 constituencies = {
          "county_name": ["constituency_name_1", "constituency_name_2", ...],
          ...
        }

  
wards = {
        "constituency_name": ["ward_name_1", "ward_name_2", ...],
        ...
      }

```

## Usage
This data can be useful in various ways, such as:

- Using it in your application to display the administrative units of Kenya.
- Visualizing the data on a map to show the different county, constituency and ward boundaries.
- Use it as a reference when working with data that is related to Kenya's geographical divisions.

## Data source
The data has been scraped from [Wikipedia](https://en.wikipedia.org/wiki/List_of_constituencies_of_Kenya)

## Disclaimer
Though a lot of effort was put to ensure the accuracy of data contained herein, the author of this repository disowns any harm resulting from reliance of this data.

## Installation
If you want to use this data in your python script, you can clone the repository and read the file as follows:

```
import json

with open("locations.txt", "r") as file:
    data = json.load(file)

print(data)
```
`The data can also be read as JSON object in Javascript or a pandas DataFrame.`

## Contributions
I welcome any contributions to this repository, whether it's adding new features or fixing errors in the data. If you would like to contribute, please submit a pull request.
Can you take the challenge of adding other administrative units such as locations, sub-locations, villages?


## Conclusion
Thank you for using this repository. We hope it will be useful in your project! If you have any questions or feedback, please feel free to open an issue.

Happy coding. Cheers!  :sunglasses:
