R package for Bit.ly & Bitly.com & j.mp and other custom domains
============
Licensed under [MIT](http://en.wikipedia.org/wiki/MIT_License)

### Help needed !!!

- Testers (with the enterprise account too). Please install and try using it. Then report bugs in <https://github.com/dmpe/rbitly/issues>


### What is/not implemented:

<http://dev.bitly.com/user_info.html>  | Implemented Yes/No
------------- | -------------
/v3/oauth/app  | (**NOT**, see below)
/v3/user/info  | Yes
/v3/user/link_history | Yes
/v3/user/network_history  | (**NOT**)
/v3/user/tracking_domain_list  | Yes

<http://dev.bitly.com/link_metrics.html>  | Implemented Yes/No
------------- | -------------
/v3/link/clicks  | Yes
/v3/link/countries  | Yes
/v3/link/encoders  | (**NOT**)
/v3/link/encoders_by_count  | Yes
/v3/link/encoders_count  | Yes
/v3/link/referrers  | (**NOT**)
/v3/link/referrers_by_domain  | (**NOT**)
/v3/link/referring_domains  | Yes


<http://dev.bitly.com/user_metrics.html> | Implemented Yes/No | Premium
------------- | ------------- | -------------
/v3/user/clicks  | Yes | NO
/v3/user/countries  | Yes | No
/v3/user/popular_earned_by_clicks  | No  | Yes
/v3/user/popular_earned_by_shortens  | No  | Yes
/v3/user/popular_links  | Maybe
/v3/user/popular_owned_by_clicks  | No  | Yes
/v3/user/popular_owned_by_shortens | No  | Yes
/v3/user/referrers  | Maybe
/v3/user/referring_domains | Maybe
/v3/user/shorten_counts | Maybe


<http://dev.bitly.com/organization_metrics.html> | Implemented Yes/No | Premium
------------- | ------------- | -------------
/v3/organization/brand_messages  | No | Yes
/v3/organization/clicks  | No | Yes
/v3/organization/intersecting_links | No  | Yes
/v3/organization/leaderboard  | No  | Yes
/v3/organization/missed_opportunities | No  | Yes
/v3/organization/popular_links | No  | Yes
/v3/organization/shorten_counts | No  | Yes


<http://dev.bitly.com/domains.html> | Implemented Yes/No | Premium
------------- | ------------- | -------------
/v3/bitly_pro_domain  | No | Yes
/v3/user/tracking_domain_clicks  | No | Yes
/v3/user/tracking_domain_shorten_counts  | No | Yes

- <http://dev.bitly.com/links.html>
    + None endpoints are implemented here. 
- <http://dev.bitly.com/nsq.html>  
    + None endpoints are implemented here. 
    
- At the moment **no OAuth support** -> only basic [HTTP Basic Authentication Flow](http://dev.bitly.com/authentication.html#basicauth), which requires `Generic Access Token` from <https://bitly.com/a/oauth_apps>

- Additionally, only a **small subset of input paramaters** has been implemented. 

### Installation

Use devtools to install the development version from Github:

```
devtools::install_github('dmpe/rbitly', build_vignettes = FALSE)
```

### How to Contribute

- Fork the repository
- Create and switch to a new branch `git checkout -b [name_of_your_new_branch]`
- Do the changes (i.e. edit files)
- Push remote branch to your github `git remote add [name_of_your_remote]` & `git push origin [name_of_your_remote]`
- Create a new pull request (to my `master` branch)

Want a direct push access? No problem, just let me know.

### Special Thanks to:

- Myself ([@dmpe](https://www.github.com/dmpe)) :yum:
- Somewhat (well, quite a lot) inspired by [Quandl Api R](https://github.com/quandl/R-package/)







