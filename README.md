# Welcome to CrossfitOpen webscraper !


I'm really excited to share my first personal project. That's why there is a lot of room for code improvement and additional functionalities.

My goal was to collect the name and nationality of the CrossFit athletes who participated the CrossFit Open 2023.


## Libraries

The I used the following:
- **time** 
- **pandas**
- **selenium**   `pip install selenium`
Using Google Chrome Driver
- **tqdm** `pip install tqdm`

## Specificity

**<u>URL<u>**
To change your research parameter you car directly change in the function `get_url` the parameter of the URL ***division=2&region=0&scaled=0***
> divison 1 = men | division 2 = women | scaled 0 = RX | scaled 1 = scaled ...
> Feel free to create a function for that.

**<u>TIME<u>**
In the function `get_content` the recommended loading time for `time.sleep(2)` is 10 seconds.
However, this will make the scraping longer. Upon you internet speed you can reduce this number. 2 seconds works fine for me.
## Run the code

    get_data_as_csv(driver_name,page_nb,'file_name_output')

**driver_name** here in the code I used google chrome as `driver`
    **page** here it's expected an integer, you can find the max page directly on the bottom page of the leaderboard CrossFit Game website.
    **'file_name_output'**   here it's expected a string for the name of the exported csv file. The file will be save in same location as **crossfitopen_webscraper.ipynb**

## Backup

If somehow you get an error during the process, a backup file will be generated with the completed iteration.
