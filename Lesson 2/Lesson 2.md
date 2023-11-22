Test-cases

UI level

Test case #1 : Checking Google searches through the search bar

Pre-conditions: Connect your device to the Internet. Open a browser. In the address bar, type www.google.com and press Enter.

Given user posts “Dualbootpartners” in the search bar

When user pushes button “Enter” on keyboard

Then Below the input line are tabs labeled "All" - active, "Images", "Maps", "News", "Videos", "More". Below the tabs, a list with links and a short description including the value "Dualbootpartners" entered in the search bar is displayed.

Given Below the input line are tabs labeled "All" - active, "Images", "Maps", "News", "Videos", "More". Below the tabs, a list with links and a short description including the value "Dualbootpartners" entered in the search bar is displayed.

When user clicks on tab “Images”

Then Below the input line, tabs named "All", "Images", "Active", "Maps", "News", "Videos", "More" are displayed. Images matching the "Dualbootpartners" value are displayed below the tabs

Given Below the input line, tabs named "All", "Images", "Active", "Maps", "News", "Videos", "More" are displayed. Images matching the "Dualbootpartners" value are displayed below the tabs

When  user clicks on tab “Maps”

Then Information about the value entered in the search box and a map with the location are displayed

Given Information about the value entered in the search box and a map with the location are displayed

When user clicks on tab “News”

Then The tabs "All", "Images", "Maps", "News" - active, "Videos", "More" are displayed below the input line. An error is displayed with the text: "Did you mean: [link] No results containing all your search terms were found. Your search - dualbootpartners - did not match any news results. Suggestions: Make sure that all words are spelled correctly. Try different keywords. Try more general keywords."

Given The tabs "All", "Images", "Maps", "News" - active, "Videos", "More" are displayed below the input line. An error is displayed with the text: "Did you mean: [link] No results containing all your search terms were found. Your search - dualbootpartners - did not match any news results. Suggestions: Make sure that all words are spelled correctly. Try different keywords. Try more general keywords."

When  user clicks on tab “Videos”

Then Below the input line are tabs labeled "All", "Images", "Maps", "News", "Videos" - active, "More". Below the tabs, videos matching the value entered in the search bar are displayed

Test-case #2: Google search  via image upload

Pre-conditions: Connect your device to the Internet. Open a browser. In the address bar, type www.google.com and press Enter.

Given The "search by image" button is clicked

When user dragged an image without text from the device into the download field

Then The uploaded image is displayed on the left, above the image is the "Find image source" button, below the image the buttons "Search" - active, "Text", "Translate", on the right is the list with links and image.

Given The uploaded image is displayed on the left, above the image is the "Find image source" button, below the image the buttons "Search" - active, "Text", "Translate", on the right is the list with links and image.

When user clicks on “Find image source”

Then An "Exact matches" button, a list with links and an image is displayed.

Given An "Exact matches" button, a list with links and an image is displayed.

When user clicks on “Exact matches”

Then The uploaded image is displayed on the left, above the image is the "Find image source" button, below the image the buttons "Search" - active, "Text", "Translate", on the right is the list with links and image.

Given The uploaded image is displayed on the left, above the image is the "Find image source" button, below the image the buttons "Search" - active, "Text", "Translate", on the right is the list with links and image.

When user clicks on “Text”

Then The uploaded image is displayed on the left, above the image the button "Find image source", below the image the buttons "Search", "Text" - active, "Translate". On the right side the error "Can't find text Try a different photo, or switch to Search" is displayed

Given The uploaded image is displayed on the left, above the image the button "Find image source", below the image the buttons "Search", "Text" - active, "Translate". On the right side the error "Can't find text Try a different photo, or switch to Search" is displayed

When user clicks on “Translate”

Then The uploaded image is displayed on the left, above the image the button "Find image source", below the image the buttons "Search", "Text" - active, "Translate". On the right side the error "Can't find text to translate Try a different photo, or switch to Search" is displayed

E2E level

Test-case #3: Search for a site in Google by name

Pre-conditions: Connect your device to the Internet. Open a browser. In the address bar, type www.google.com and press Enter.


Given user posts “Dualbootpartners” in the search bar

When user pushes button “Enter” on keyboard

Then Below the input line are tabs labeled "All" - active, "Images", "Maps", "News", "Videos", "More". Below the tabs, a list with links and a brief description including the value "Dualboot partners" entered in the search bar is displayed.

Given Below the input line are tabs labeled "All" - active, "Images", "Maps", "News", "Videos", "More". Below the tabs, a list with links and a brief description including the value "Dualboot partners" entered in the search bar is displayed.

When user click on “cross” button in the search bar

Then search bar is empty

Given search bar is empty

When user types “Dualboot”

Then A drop-down list with values matching the entered "Dualboot" value was opened

Given A drop-down list with values matching the entered "Dualboot" value was opened

When user clicks on “Dualboot partners” from drop-down list

Then Below the input line are tabs labeled "All" - active, "Images", "Maps", "News", "Videos", "More". Below the tabs, a list with links and a brief description including the value "Dualboot partners" entered in the search bar is displayed.

Given Below the input line are tabs labeled "All" - active, "Images", "Maps", "News", "Videos", "More". Below the tabs, a list with links and a brief description including the value "Dualboot partners" entered in the search bar is displayed.

When user click on first link in list

Then https://dualbootpartners.com/ site is opened

Test-case #4: Search for a photo in Google

Pre-conditions: Connect your device to the Internet. Open a browser. In the address bar, type www.google.com and press Enter.


Given user posts “Dualbootpartners” in the search bar

When user pushes button “Enter” on keyboard

Then Below the input line are tabs labeled "All" - active, "Images", "Maps", "News", "Videos", "More". Below the tabs, a list with links and a brief description including the value "Dualboot partners" entered in the search bar is displayed.

Given Below the input line are tabs labeled "All" - active, "Images", "Maps", "News", "Videos", "More". Below the tabs, a list with links and a brief description including the value "Dualboot partners" entered in the search bar is displayed.

When users clicks on “Images” tab

Then Below the input line, tabs named "All", "Images", "Active", "Maps", "News", "Videos", "More" are displayed. Below the tabs, images matching the value entered in the search bar are displayed

Given Below the input line, tabs named "All", "Images", "Active", "Maps", "News", "Videos", "More" are displayed. Below the tabs, images matching the value entered in the search bar are displayed

When user clicks on any image

Then The image is marked as selected, a larger image appears on the right with a link

Given The image is marked as selected, a larger image appears on the right with a link

When user click on link under the selected image

Then The site indicated in the link has opened

Integration level


Test-case #5: Check integration between Google and components

Pre-conditions: Connect your device to the Internet. Open a browser. In the address bar, type www.google.com and press Enter.

Given user posts “Dualboot partners” in the search bar

When user pushes button “Enter” on keyboard

Then The value "Dualboot partners" is fully passed to the search query

Given user posts “+_0@±±§” in the search bar

When user pushes button “Enter” on keyboard

Then The value "+_0@±±§" is fully passed to the search query


Given The value "+_0@±±§" is fully passed to the search query

When users posts “Dual”  in the search bar

Then A drop-down list with values matching the entered "Dual" value was opened
Given user posts “Dualboot partners” in the search bar

When user pushes button “Enter” on keyboard

Then Search results are integrated and are a combination of web pages, images, videos and other types of content relevant to the query.

Given “Images” tab is clicked and user posts “Dualboot partners” in the search bar

When user clicks on “Enter” on keyboard

Then Image search results are displayed that fit seamlessly into the search interface.


Test-case #6: Search for News in Google

Pre-conditions: Connect your device to the Internet. Open a browser. In the address bar, type www.google.com and press Enter.

Given user posts “Global Economy” in the search bar

When user clicks on Enter

Then News search results are displayed on the screen, blending seamlessly into the search interface

Given user posts “Instagram” in the search bar

When user clicks on Enter

Then Ads are integrated into the search results page and clearly labeled as sponsored content

Given Change the language setting to Russian and enter  “Глобальная Экономика” in search bar

When user clicks on Enter

Then Search results and interface elements are displayed in the selected language, indicating proper localization integration.






