Releasing this little helper i've done for a warehouse management dashboard.

- F*king awesome to use for EAN type of barcode scaners
- Or just plain keyboard inputs

Use case:
- you register a string and the callback function
- when the string is being entered on the keyboard or any input devise such as scaners will trigger callback

Usage:
$(window).keyCombo('next', function{
    // do something here when 'next' is pressed in sequence
});

// to use object listeral
// careful, this example uses window scope
// edit to your own scope
// and you can hook it to your plugin nameapce
// eg: your.plugin.scaner = scaner('scope', {string:callback})

scaner('window', {
    'Next': function(){
        // do something when next is scanned
    }
    , 'prev': function(){
    
    }
})

