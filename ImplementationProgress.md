### What is/not implemented:

Based on <http://dev.bitly.com/>

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
/v3/link/encoders  | Yes
/v3/link/encoders_by_count  | Yes
/v3/link/encoders_count  | Yes
/v3/link/referrers  | Yes
/v3/link/referrers_by_domain  | Yes
/v3/link/referring_domains  | Yes


<http://dev.bitly.com/user_metrics.html> | Implemented Yes/No | Premium
------------- | ------------- | -------------
/v3/user/clicks  | Yes 
/v3/user/countries  | Yes 
/v3/user/popular_earned_by_clicks  | No  | Yes
/v3/user/popular_earned_by_shortens  | No  | Yes
/v3/user/popular_links  | Yes
/v3/user/popular_owned_by_clicks  | No  | Yes
/v3/user/popular_owned_by_shortens | No  | Yes
/v3/user/referrers  | Yes
/v3/user/referring_domains | Yes
/v3/user/shorten_counts | Yes


<http://dev.bitly.com/domains.html> | Implemented Yes/No | Premium
------------- | ------------- | -------------
/v3/bitly_pro_domain  | Yes| No
/v3/user/tracking_domain_clicks  | No | Yes (cannot do unless sombody helps)
/v3/user/tracking_domain_shorten_counts  | No | Yes (cannot do unless sombody helps)


- <http://dev.bitly.com/links.html>
    + None endpoints are implemented here, because there is no use-case from my point of view. Per request can implement, however. 
    
- <http://dev.bitly.com/nsq.html>  
    + None endpoints are implemented here, because all are premium. 
    
- <http://dev.bitly.com/organization_metrics.html>
    + None endpoints are implemented here, because all are premium.

- At the moment **no OAuth support** -> only basic [HTTP Basic Authentication Flow](http://dev.bitly.com/authentication.html#basicauth), which requires `Generic Access Token` from <https://bitly.com/a/oauth_apps>

- Additionally, only a **small subset of input paramaters** has been implemented. 