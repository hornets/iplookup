#IP Lookup
This script trys to make http://ip-api.com/json/ looks better on a daily use. 

The desktop view has a map on the bottom showing the current location of the ip. The mobile version is responsive without map and github banner

##Demo
https://iplook.herokuapp.com or [iplook.tk](http://iplook.tk)

##Setup
First, get an mapID. My mapID is just a demo and will eventually run out of the free limit.

1. Go to https://www.mapbox.com/
2. Create a map
3. Click 'Share' -> 'Developer' and there is your mapId
4. Go to ```config.py``` and put your mapid there.

Then setup virtual environment

```
virtualenv ev
source ev/bin/activate
```

Install Dependencies

```
pip install -r requirements.txt
```

Run

```
python main.py
```

It will then run on http://localhost:5000

Enjoy

:)

##API
Besides the current ip address the visitor is visiting this web app from, one can also do 

```
http://hostingAddress/ipAddress
```

to get the info about a a specific ip address, or

```
http://hostingAddress/domainName
```

##Credits
The backend API is powered by [IP Geolocation API](http://ip-api.com/docs/). They provide free usage of their API for non-commercial use.

The template is [Bootstrap](http://getbootstrap.com/).

The color of the text is 紅(kurenai) from [Nippon Colors](http://nipponcolors.com/#kurenai).

The map is created in [Mapbox](https://www.mapbox.com/).

The web framework used is [Flask](http://flask.pocoo.org/).

##License
```
The MIT License (MIT)

Copyright (c) 2013 (Paul) Jianer Shi (hipaulshi@gmail.com)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/paulshi/iplookup/trend.png)](https://bitdeli.com/free "Bitdeli Badge")