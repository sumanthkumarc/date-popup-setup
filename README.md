# date-popup-setup
This repo has necessary files to be included and code to get you started with date time popup in a jiffy!!

1. Include all js and css files given in repo.
2. Make sure you include bootstrap-datetimepicker.min.js at the end of all js files ie., the script tag which includes this js file should be at end of other script tags which include other js files like collapse.js etc.
3. invoke the datetimepicker() on wanted element.

   jQuery('#element').datetimepicker({
           format: 'D.MM.YYYY - HH:mm',
           useCurrent : false,
           showTodayButton : true
    });
