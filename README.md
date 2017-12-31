# DEPRECATED *** Use [angular-google-place](https://github.com/psykolm22/angular-google-place/) ***



# Issues have been moved to new repo : [angular-google-place](https://github.com/psykolm22/angular-google-place/)
# n2-google-place-autocomplete is now available as [angular-google-place](https://github.com/psykolm22/angular-google-place/)




# ng2-google-place-autocomplete
This is a Google-Autocomplete Module for Angular.

[![NPM](https://nodei.co/npm/ng2-google-place-autocomplete.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/ng2-google-place-autocomplete/)

# Build with angular-cli 1.0.0-beta.31 and @angular 2.4.7

[![CircleCI](https://circleci.com/gh/psykolm22/ng2-google-place-autocomplete.svg?style=shield&circle-token=cf5e1c8f08d7d90c845e41ba20df0c8a6fc38892)](https://github.com/psykolm22/ng2-google-place-autocomplete) [![devDependency Status](https://gemnasium.com/badges/github.com/psykolm22/ng2-google-place-autocomplete.svg)](https://gemnasium.com/github.com/psykolm22/ng2-google-place-autocomplete) [![npm](http://img.shields.io/npm/v/ng2-google-place-autocomplete.svg?style=flat)](https://www.npmjs.org/package/ng2-google-place-autocomplete) [![license](https://img.shields.io/github/license/psykolm22/ng2-google-place-autocomplete.svg)]()

[Docs](https://psykolm22.github.io/ng2-google-place-autocomplete) | [Demo](https://psykolm22.github.io/) 

# GitHub
Please feel free to declare issues or contribute  : https://github.com/psykolm22/ng2-google-place-autocomplete

# What about next Improvements ? 
Visit our [Board](https://github.com/psykolm22/ng2-google-place-autocomplete/projects/1)
# Installation

NPM

    npm install --save ng2-google-place-autocomplete

YARN

    yarn add ng2-google-place-autocomplete --save

# Don't forget to add google api in your index.html
* in your index.html:
```html
<script  type="text/javascript" src="https://maps.googleapis.com/maps/api/js?libraries=places"></script>
```

# Usage
* Use it in your HTML elements, for example:
```html
<input type="text" [(ngModel)] = "address" 
 [options]='options' 
 (setAddress) = "getAddress($event)"
 (street_number) = 'street_number=$event'
 (street)= 'street=$event'
 (city)= 'city=$event'
 (state)='state=$event'
 (district)='district=$event'
 (country)='country=$event'
 (postal_code)='postal_code=$event'
 (lat)='lat=$event' 
 (lng)='lng=$event' 
 (adr_address)='adr_address=$event' 
 (name)='name=$event' 
 (place_id)='place_id=$event' 
 (types)='types=$event' 
 (url)='url=$event'  
 (utc_offset)='utc_offset=$event' 
 (vicinity)='vicinity=$event' 
 (photos)='photos=$event' 
 (airport)='airport=$event' 
 (CountryCodes)='CountryCodes=$event'
  id="autocomplete"
 ng2-google-place-autocomplete/> 
```


* Add GooglePlaceModule in your app.module.ts:
```typeScript
import {GooglePlaceModule} from 'ng2-google-place-autocomplete';

@NgModule({
    ...
    import: [..., GooglePlaceModule]
})
```

#Options
Options for Google Search
* Choose one type from
```
  [ '(cities)', '(regions)', 'country', 'postal_code', 'sublocality', 'establishment', 'address', 'geocode'] 
```  
* country ( dynamic change allow) : CountryCode ISO 3166-1 Alpha-2 ( see demo )
```html  
[options]="{
    types: [],
    componentRestrictions: { country: 'FR' }
    }"
```
#Tested in:
* Chrome
* Firefox
* Safari


#For AngularJS:
https://github.com/vskosp/vsGoogleAutocomplete




