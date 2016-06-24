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

#Dropdown Menus

### Flush with Top (for search results and filtering options)

To display results/options add a ul below the `<input>` or `<a>` tag and add the class `.mls-dropdown-flush` to the parent element

<!-- Full width inputs add the class of mls-input-full -->

####example — searchbar


<div class="input-group mls-input-full mls-input-results">

  <input type="text" class="form-control" placeholder="Username" aria-describedby="basic-addon1">

  <ul>
    <li></li>
    <li></li>
    <li></li>
  </ul>

</div>


####example — dropdown button
<div class="btn-group" role="group">
    <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Dropdown
     <span class="caret"></span>
     </button>
     <ul class="dropdown-menu">
         <li><a href="#">Result</a></li>
         <li><a href="#">Result</a></li>
     </ul>
   </div>

here's the bootstrap for dropdown

<div class="dropdown">
  <button class="btn btn-default dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown" aria-haspopup="true" aria-expanded="true">
    Dropdown
    <span class="caret"></span>
  </button>
  <ul class="dropdown-menu" aria-labelledby="dropdownMenu1">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>
</div>



#Filtering 

There are three types of filters: date-range-selectors, possible options, and search.

these are represented by the classes ```mls-filter-date```, ```mls-filter-options```, ```mls-filter-search```

<!-- filtering by date add the class of mls-filter-date -->
   
**this one is tricky — we have two kinds of dropdowns with two different kinds of results.  

<div class="sorting-and-filtering-header">
   <div class="btn-drop-down-container">
   <a class="mls-btn-popup" href="" title="">Story Date</a>
   <ul class="dropdown-menu" aria-labelledby="dropdownMenu1">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>
  </div>
  <div class="btn-group" role="group">
    <button type="button" class="btn btn-default dropdown-toggle" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Dropdown
     <span class="caret"></span>
     </button>
     <ul class="dropdown-menu">
         <li><a href="#">Result</a></li>
         <li><a href="#">Result</a></li>
     </ul>
   </div>
</div>

# Story Card

```
<div class="mls-card">
    <h1>
    <h2>
</div> ```



## Story Card State

Cards can be unread or _important_ and can be chagned using classes.

```
<div class="mls-card mls-card-is-unread">
    ...
</div>

<div class="mls-card mls-card-is-important">
    ...
</div>
```


<div class="autocomplete-input has-results">
    <input type="text" />
    <ul class="autocomplete-results-list">
        ...
    </ul>
</div>

# Dropdowns


<ul class="dropdown-menu mls-popover" aria-labelledby="dropdownMenu1">
    <li><a href="#">Action</a></li>
    <li><a href="#">Another action</a></li>
    <li><a href="#">Something else here</a></li>
    <li role="separator" class="divider"></li>
    <li><a href="#">Separated link</a></li>
  </ul>

  .mls-popover {

      shadow,
      border-radius


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

