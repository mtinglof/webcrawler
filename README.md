# Webcrawler
> My first attempt at creating a program to collect soccer player data 

This is program is a quick way to scrap soccer statistics off the site whoscored.com. The program is specifically designed to navigate the sites JavaScript and compile the wanted data into a readable format. 

## Installing / Getting started
This program was coded in Python Version 3.6 
In addition to the latest version of Python, several packages are needed before the application can be executed.

```
pip install beautifulsoup4
pip install numpy
pip install pandas
pip install selenium
```

### Initial Configuration

A Chrome Driver is used to scrap data from the web. It is required that the Chrome Driver is saved to your local machine and the path is properly set in the program. More information about the Chrome Driver can be found here http://chromedriver.chromium.org/getting-started 

It is also recommended that you configure the AdBlock extension for the ChromeDriver. More information can be found here https://stackoverflow.com/questions/42231604/how-to-activate-adblocker-in-chrome-using-selenium-webdriver and the path to the extension should be set within the program. 

## Features

The program itself is very versatile, with much of the functionality focused on data manipulation with excel files. Two out of the three classes within the program are designed to assign personalized weight systems to the collect data as well as create optimized lists of players based on a per determined criteria. In addition, a very rudimentary completion timer is implemented. 

#### Argument 1
Type: `String`  

Pass the site you wish to scrap from. Initially the site used was whoscored.com

Example:
```
GameDay("https://www.whoscored.com/") 
```

#### Argument 2
Type: `String`  

File name, initially configured for .xlsx file 

Example:
```
GameDay("https://www.whoscored.com/", "mmb") 
```

#### Argument 3
Type: `String`  

Sets the weight type for data collected. Can be set to string "yes" or "no" 

Example:
```
GameDay("https://www.whoscored.com/", "mmb", "yes") 
```

## Contributing

Pull requests are gladly accepted. Parts of the code can be used for other WebCrawlers however the specific nature of the code makes it difficult to repurpose the entirety. Future commits may include creating a more robust and versatile application that can scrap from more than one site. If you would like to contribute to the project, please fork the repository and use a feature branch. 

## Links

- Repository: https://github.com/mtinglof/webcrawler
- Chrome Driver: http://chromedriver.chromium.org/getting-started 
- AdBlock Extension: https://stackoverflow.com/questions/42231604/how-to-activate-adblocker-in-chrome-using-selenium-webdriver
- My Homepage: https://github.com/mtinglof

## Licensing

This project is licensed under Unlicense license. This license does not require
you to take the license with you to your project.
