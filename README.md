jQuery-CoreUISelect
===================

jQuery CoreUISelect is a cross browser easy to stylize select element with jQuery and CSS

## Available Features:

* Full customization
* Automatic calculations
* Keyboard support
* Powerful callback functions
* Compatible with mobile devices
* Support jScrollPane plugin for customize default scrollbar

## Default settings
    $('#countries').CoreUISelect();

## With jScrollPane plugin
    $('#countries_2').CoreUISelect({
        jScrollPane : {
           verticalDragMinHeight: 20,
           verticalDragMaxHeight: 20,
           showArrows : true
        }
     });
    
## Append to body setting
Custom dropdown build in body

    $('#countries_3').CoreUISelect({
        appendToBody : true
    });

## Callback functions
Custom dropdown build in body

    $('.b-core-ui-select__select').CoreUISelect({
         onInit : addCoreUISelectListener,
         onOpen : addCoreUISelectListener,
         onClose : addCoreUISelectListener,
         onChange : addCoreUISelectListener,
         onDestroy : addCoreUISelectListener
     });
         
     function addCoreUISelectListener(select, event){
         console.log(el, event);
     } 