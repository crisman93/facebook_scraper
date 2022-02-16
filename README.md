# Facebook Scraper

The functions in this scraper are based on this [facebook-scraper](https://github.com/kevinzg/facebook-scraper). 

## Installation requirements

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install facebook-scraper.
```bash
pip install facebook-scraper
```
Function requires cookies to be passed in as an argument. To collect cookies in chrome download this [cookies extension](https://chrome.google.com/webstore/detail/get-cookiestxt/bgaddhkoddajcdgocldbbfleckgcbcid). To collect cookies in Firefox download this [cookies extension](https://addons.mozilla.org/en-US/firefox/addon/cookie-quick-manager/). Make sure that you include both the c_user cookie and the xs cookie, you will get an InvalidCookies exception if you don't.

## Usage

```python
from facebook_scraper import get_posts
import pandas as pd

comments = scrape_comments(fb_group_list, 50, cookies, {"comments": True, "allow_extra_requests": True, 'posts_per_page': 1})
```

## License
