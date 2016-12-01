# date-popup-setup
This repo has necessary files to be included and code to get you started with date time popup in a jiffy!!
This plugin used is bootstrap date time picker by Eonasdan. See below links.
<br />

Links: 
<ul>
<li>https://github.com/Eonasdan/bootstrap-datetimepicker</li>
<li> http://eonasdan.github.io/bootstrap-datetimepicker</li>
</ul>
Steps:
1. Include all js and css files given in repo.
2. Make sure you include bootstrap-datetimepicker.min.js at the end of all js files ie., the script tag which includes this js file should be at end of other script tags which include other js files like collapse.js etc.
3. invoke the datetimepicker() on wanted element.


```
   jQuery('#element').datetimepicker({
           format: 'D.MM.YYYY - HH:mm',
           useCurrent : false,
           showTodayButton : true
   });
```
<br />

In any case , if you want the popup to stay open, always, add the property debug: true.
```
   jQuery('#element').datetimepicker({
           debug: true
   });
```
<br />
The below code tries to automatically open time picker when a date is clicked. taken from issue filed at below url:
https://github.com/Eonasdan/bootstrap-datetimepicker/issues/1368
```   
       jQuery('#element')
                .on("dp.show", function (e) {
                    $(".day").on('click', function () {
                        $("a[data-action='togglePicker']").trigger('click');
                    });
                })
                .on("dp.change", function (e) {
                    $(".day").on('click', function () {
                        $("a[data-action='togglePicker']").trigger('click');
                    });
                })
```                
