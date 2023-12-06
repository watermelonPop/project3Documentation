# Home

Home page for customers, contains image slide shows and all of the drinks with the drink names, descriptions, and images

## Methods

<!-- @vuese:Home:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|nextSlide|Click to the next slide of the slideshow of drink images|-|
|prevSlide|Click to the previous slide of the slideshow of drink images|-|
|startAutoSlide|Begin the slideshow of images from the drink menu|-|
|fetchOrderHistoryData|Retrieve order history of drink items ordered based on user date inputs from the database|-|
|fetchMenuData|Retrieve all menu drink items from the menu sql table of the database to be displayed on the home page|-|
|addFrequencies|Based upon the order history of the drinks a frequency of drinks ordered is calculated to display on the homepage|-|
|findPopular|Finalize a list of most popular drinks ordered by other customers on the homepage|-|
|fetchAltText|Retrieved image alt text from the database and image table|-|
|getAltText|Retrieve boba tea image descriptions and images|-|
|togglePopular|Enable the calculation of popular drinks on the home page|-|
|toggleHover|Allow hovering over the popular drinks on the home page|-|
|getLocation|Retrieve location of the user accessing the website to enable the weather API of their location|-|
|showPosition|Retrieve the weather based on the location of the user accessing the website|-|
|fetchWeather|Retrieve weather data based on the longitude and latitude coordinates|-|
|applyFontSize|Apply the font size designated by the user on the website page|-|

<!-- @vuese:Home:methods:end -->


## Computed

<!-- @vuese:Home:computed:start -->
|Computed|Type|Description|From Store|
|---|---|---|---|
|endDate|-|Generate end date based upon user input to find popular items ordered|No|
|startDate|-|Generate start date based upon user input to find popular items ordered|No|
|visiblePopular|-|Find popular drink items based on the dates inputted by the user|No|

<!-- @vuese:Home:computed:end -->


