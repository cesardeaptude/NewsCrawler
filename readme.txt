-------------------------------------------
NewsCrawler

A news crawler for the site tehrantimes.com
-------------------------------------------
Prerequsites

Python3 and beautifulsoup library installed
-------------------------------------------
Usage

The main file (app.py) has commented the four functionalities (get_links, get_elements, get_previews and finder)
you can uncomment each block to see how it works.

get_links
This functionality get only the links of the preeliminary views of the news (is recommendable that you open the
sites used to test it to see what elements are given), it accept multiple links and return back a list of list 
of links for each site in the args.

get_elements
This functionality get the elements (topic, author, title, date, image, text, related_news, tags) of a given news 
site or multiple sites you can uncomment the # for test it with multiple sites, it gives you a list of list for 
each news given in the args.

get_previews
This functionality gives you the elements of the preview of the news, it is tested with the same links of the
get_links functionality, it accept several links but it accept parameters, it create the querystring with those
parameters and obtain the elements of the previews of the news.

finder
This is like a search engine, you give it a keyword list and some parameters and gives you the elements of all
those news that contain the keyword list, it is still NOT finished.
------------------------------------------------------------------------------------------------------------------
The file test_appunitest execute unitary test for each functionality 

For get_links there are two test, one is for test if the list of links given have the correct number of elements
and the second is to test that all the links given are not empty and start with the domain name of the site 
(https://www.tehrantimes.com/).

For get_elements it only test if the number of elements of the list given is correct.

For get_previews it execute two test, as it gives you a list of list, it test first the longitude of the main list
later it test the longitude of each intern list.

For finder the unit test is not finished.
