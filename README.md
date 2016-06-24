# Buttons

Main buttons are anchor tags and inherit `.mls-btn`.


<!-- Base buttons add the class of mls-btn -->
```<a class="mls-btn" href="#">Example</a>```

<!-- Large buttons add the class of mls-btn-lg -->
```<a class="mls-btn mls-btn-lg" href="#">Example</a>```

<!-- Medium buttons add the class of mls-btn-lg -->
```<a class="mls-btn mls-btn-lg" href="#">Example</a>```

<!-- Small buttons add the class of mls-btn-lg -->
```<a class="mls-btn mls-btn-lg" href="#">Example</a>```

<!-- Group buttons add the class of mls-btn-group to a UL tag -->
```<ul class="mls-btn mls-btn-group" href="#">Example</ul>```


Context Buttons are anchor tags and use the class `.mls-context-btn`.

<!-- Context buttons add the class of mls-btn-context -->
```
<a class="mls-popup-btn" href="" title="">Unread</a>
```

# Inputs 

### General Inputs
Inputs are pulled from bootstrap and modified with the class `.mls-input`.

```
<div class="input-group mls-input">
  <input type="text" class="form-control" placeholder="Username" aria-describedby="basic-addon1">
</div>
```

<!-- Full width inputs add the class of mls-input-full -->

```
<div class="input-group mls-input-full">
  <input type="text" class="form-control" placeholder="Username" aria-describedby="basic-addon1">
</div>
```

<!-- Large inputs add the class of mls-input-lg-->

```
<div class="input-group mls-input-lg">
  <input type="text" class="form-control" placeholder="Username" aria-describedby="basic-addon1">
</div>
```

<!-- Small inputs add the class of mls-input-sm-->

```
<div class="input-group mls-input-sm">
  <input type="text" class="form-control" placeholder="Username" aria-describedby="basic-addon1">
</div>
```

### Input Textarea

textarea tags are tricky in bootstrap because it has a tendency to ignore the "rows" attribute. however if you put it in a div and then ignore the form-group-(x) call within the first div, the rows and the cols can be controlled within the textarea. 

<!-- Textarea tags add the class of mls-textarea to modify it's styles -->
```
<div class="form-group mls-textarea">
    <textarea class="form-control" rows="8"></textarea>
</div>
```

#Modals

Modals are div tags and inherit `.mls-modal`. Although they have set widths, their height is always auto (set by the content).

<!-- Large modals add the class of mls-modal-lg -->
```<div class="mls-modal mls-modal-lg">Example</div>```

<!-- Medium modals add the class of mls-modal-md -->
```<div class="mls-modal mls-modal-md">Example</div>```

<!-- Small modals add the class of mls-modal-sm -->
```<div class="mls-modal mls-modal-sm">Example</div>```

###Modal Curtain

.mls-modal .mls-curtain will add a backdrop behind the modal but above the content — whenever a modal is triggered.

```<div class="mls-curtain"></div>```


###Popups/Tooltips

Popups/Tooltips are div tags and inherit `.mls-popup`

<!-- Base style popups use the class of mls-popup -->
```
<div class="mls-popup"></div>
```

#Dropdowns

### Flush with Top (for search results and filtering options)

To display results/options add a ul below the `<input>` or `<a>` tag and add the class `.mls-dropdown-flush` to the parent element

####example — searchbar dropdown results
```
<div class="input-group mls-input-full .mls-dropdown-flush">
  <input type="text" class="form-control" placeholder="Username" aria-describedby="basic-addon1">
  <ul>
    <li><a href="#">Result</a></li>
    <li><a href="#">Result</a></li>
    <li><a href="#">Result</a></li>
  </ul>
</div>
```
### Separate from button (not flush)

 To display a popup menu we use our custom we use the bootstrap component, but replace their button with our own `<a class="mls-btn-popup" href="" title="">Story Date</a>` and then add `.mls-dropdown-separate` to the parent element (container element)

####example — dropdown menu
```
<div class="btn-group mls-dropdown-separate" role="group">
  <a class="mls-btn-popup" href="" title="">Story Date</a>
  <ul class="dropdown-menu">
    <li><a href="#">menu-item</a></li>
    <li><a href="#">menu-item</a></li>
  </ul>
</div>
```

#Filtering 

There are three types of filters: date-range-selectors, possible options (brand & region), and search.

these are represented by the classes ```mls-filter-date```, ```mls-filter-options```, ```mls-filter-search```

<!-- filtering by date add the class of mls-filter-date -->
##### Options (brand & region)   
To add filtering by Brand or Region we use the bootstrap component but our own `<ul>` class of `.mls-dropdown-flush` and add the class of `.mls-filter-options` to the parent element (container).
```
<div class="dropdown mls-filter-options">
  <button class="btn btn-default dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown" aria-haspopup="true" aria-expanded="true">
    Dropdown
    <span class="caret"></span>
  </button>
  <ul class="mls-dropdown-flush" aria-labelledby="dropdownMenu1">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>
</div>
```
##### Search 
To add filtering by search we reuse our input class `mls-input-sm` and ul class `dropdown-dropdown-flush`
```
<div class="input-group mls-input-sm">
  <input type="text" class="form-control" placeholder="Username" aria-describedby="basic-addon1">
  <ul class="mls-dropdown-flush" aria-labelledby="dropdownMenu1">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>
</div>
```

##### Date (Cris to decide how to do this)

# Story Card
Story Cards inherit the class `.mls-card`
```
<div class="mls-card">
    <h4></h4>
    <p></p>
    <h5></h5>
</div> 
```

##### Story Card State

Cards can be unread or _important_ and can be chagned using classes.

```
<div class="mls-card mls-card-is-unread">
    ...
</div>

<div class="mls-card mls-card-is-important">
    ...
</div>
```

#Asset Uploading

assets are contained in `<div>` tags and inherit the class `.mls-asset` — inside everything is custom except for the bootstrap progress bar.
```
<div class="mls-asset">
  <img src="" alt="">
  <h4></h4>
  <div class="progress">
  <div class="progress-bar" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100" style="width: 60%;">
    <span class="sr-only">60% Complete</span>
  </div>
</div>
</div>
```
there are two additional classes for successful and failed attempts at uploading `.mls-asset-success` `.mls-asset-fail`
ex. 
```
<div class="mls-asset mls-asset-fail">
 ...
</div>
```
#Pills

Pills are `<span>` tags and inherit the class `.mls-pill`

```<span class="mls-pill"></span>```

To create a brand pill add on a brand class (there is one for each)

```<span class="mls-pill mls-pill-msc"></span>```

#status-labels

Status Labels are `<span>` tags and inherit the class `.mls-status`

```<span class="mls-status"></span>```

To add a status to the label apply an additional status class to it, there are: `.mls-status-working`, `.mls-status-new`, `.mls-status-new`, `.mls-status-rejected`

```<span class="mls-status mls-status-working"></span>```

.badge {

    ...

    }

.badge .is-selected {

    ...

    }

.pill .is-selected {

    }

.is-selected {

    }

