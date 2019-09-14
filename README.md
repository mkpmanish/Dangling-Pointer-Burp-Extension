# dangling-pointer-burp-extension

This extension is a attempt to ease finding referer header related issues in a web application which usually leaks details like below

* password reset tokens
* transcation/payment receipts
* user details in url and many more occurances

## why the name is so ? 
Read yourself and see if you can figureout [https://en.wikipedia.org/wiki/Dangling_pointer](https://en.wikipedia.org/wiki/Dangling_pointer)

## Installation

Extension is written in python and hence ends Jython support to run it.

* download Jython from [here](http://search.maven.org/remotecontent?filepath=org/python/jython-standalone/2.7.1/jython-standalone-2.7.1.jar)
* Get burp professional version
* Go to Extender >> Extensions >> Add >> Browse to downloaded python file and extension will be loaded

## Working (Screenshots)
To use the extension setup the extension as shown in below gif. Then browse the application in target and go through all functionality like login/logout/order placement/forgot password etc. Once done go to extension tab and Click on **run** ( make sure you have added target domain in code/text box) we will have list of probable suspects for bugs.

##### **Add Extension** :- 
![Add Extension](https://github.com/mkpmanish/Dangling-Pointer-Burp-Extension/blob/master/dangling_1.png)

##### **Loaded Extension** :- 
![Add Extension](https://github.com/mkpmanish/Dangling-Pointer-Burp-Extension/blob/master/dangling_2.png)

##### **Extension UI** :- 
![Add Extension](https://github.com/mkpmanish/Dangling-Pointer-Burp-Extension/blob/master/dangling_3.png)

##### **Working Extension**:- 
![Add Extension](https://github.com/mkpmanish/Dangling-Pointer-Burp-Extension/blob/master/dangling_4.png)

##### **Working Extensions** :- 
![Github.com working Extension](https://github.com/mkpmanish/Dangling-Pointer-Burp-Extension/blob/master/dangling_5.png)


##### Working Video :-
![Working Extension](https://github.com/mkpmanish/dangling-pointer-burp-extension/blob/master/how_2_use_video.gif)


## Whats Next ?
* Add Logic to flag possible suspects
* Add coloring for possible bugs (High - Red/ Medium - Brown/ Low - Green/ Informational - None)
* ~~Add text box for adding target domain~~


## Credits

Thanks to [PortSwigger](https://github.com/portswigger/site-map-extractor) for this extension ( and people who wrote that extension or gave input ) without which the one which i wrote would not have been possible.

