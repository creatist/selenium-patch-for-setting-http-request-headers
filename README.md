# selenium-patch-for-setting-http-request-headers
Patchs for setting http request headers when using selenium PhantomJS Webdriver to scratch some webpage.
I use it to  modify the request headers in response to the restrictions on machine spiders.
Your application demo should use it like this,very simple:


driver =  webdriver.PhantomJS()

headers={"User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:44.0) Gecko/20100101 Firefox/44.0"}
driver.get(url,headers=headers)   //just add a headers argument in get() function,the headers argument should be a dict
             
You can see the related demo in my another repository named Star-Spider, in file sephbrowser.py ,class SePhBrowser,function get.

Please forgive me for my poor English.
