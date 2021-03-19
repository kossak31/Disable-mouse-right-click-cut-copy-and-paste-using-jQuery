# Disable-mouse-right-click-cut-copy-and-paste-using-jQuery
Disable mouse right click, cut, copy and paste using jQuery

## Disable Mouse Right Click
```javascript
<script type="text/javascript">
$(document).ready(function () {
    //Disable full page
    $("body").on("contextmenu",function(e){
        return false;
    });
    
    //Disable part of page
    $("#id").on("contextmenu",function(e){
        return false;
    });
});
</script>
```

## Disable Cut Copy & Paste
```javascript
<script type="text/javascript">
$(document).ready(function () {
    //Disable full page
    $('body').bind('cut copy paste', function (e) {
        e.preventDefault();
    });
    
    //Disable part of page
    $('#id').bind('cut copy paste', function (e) {
        e.preventDefault();
    });
});
</script>
```

## Disable Cut Copy & Paste and Right click
```javascript
<script type="text/javascript">
$(document).ready(function () {
    //Disable cut copy paste
    $('body').bind('cut copy paste', function (e) {
        e.preventDefault();
    });
   
    //Disable mouse right click
    $("body").on("contextmenu",function(e){
        return false;
    });
});
</script>
```
