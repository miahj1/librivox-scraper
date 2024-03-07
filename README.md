# Librivox Scraper
<div align="center">
    <picture><img alt="librivox logo" src="https://github.com/miahj1/librivox-scraper/assets/84815985/0dfeef48-0e54-4f22-bf7a-f1b2511751b8"></picture>
    <div align="center"><a href="https://librivox.org">Homepage</a> | <a href="https://librivox.org/search?primary_key=1&search_category=language&search_page=1&search_form=get_results">Latest Audiobooks</a></div>
</div>
<br>

LibriVox aims to offer free audio recordings of public domain books narrated by volunteers, operating as a non-commercial project with recordings donated to the public domain where texts are sourced primarily from Project Gutenberg.

## Python Modules
- Requests
- Beautiful Soup 4
- Pandas

## Summary
The client wanted the following data scraped from the website: title, author, main description, link 1 (download link), link 2 (website's url to the audiobook), language, genre, and catalog date. I've included screenshots of the elements with red rectangles below.

<picture><img src="https://github.com/miahj1/librivox-scraper/assets/84815985/5f30aefe-0b76-4862-a09a-bb855a070484"></picture>
<picture><img src="https://github.com/miahj1/librivox-scraper/assets/84815985/201958dc-4771-46ea-a0fa-9562d03099c6"></picture>
<picture><img src="https://github.com/miahj1/librivox-scraper/assets/84815985/0af44e0e-9f03-4235-b26c-c852e4b81e3b"></picture>

After collecting all the data, the client also wanted the data to be heavily pre-processed as follows: 
- Removal of single quotation `'` and backslash `\` from the titles of the books.
- Removal of `by` from the titles of the audiobooks e.g. the title would look like this for certain books `Book Title by Book Author`.
- Client's team manually listed books into a CSV with 4,000 titles: they wanted me to compare the titles already there and remove them.
- The data collected also had many duplicate URLS leading to the same book, so I grouped them into one cell where titles are comma seperated.

## Data Preview
<picture><img src="https://github.com/miahj1/librivox-scraper/assets/84815985/d7aa2969-947b-4fd3-8e2f-fc93c645987e"></picture>

## Client Feedback
