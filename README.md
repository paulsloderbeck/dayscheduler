# dayscheduler

This day scheduler app uses jQuery to dynamically render a 9-5 Calendar Scheduling app. The renderCal function uses a for loop to iterate over an array of strings for each hour. For each hour in the string a row is created in bootstrap with columns for the hour, text input, and save box. These are styled with CSS. The entire row is then appended to the container.

The scheduler saves text entered into the text area of each hour block using local storage. The rows are created dynamically with a data-hour attribute. They save button click listeners are created within the for loop for each button, and they set the value of the hour and text with the dat-hour to designate the time. The getTasks and storeTasks functions use stringify and parse to retreive and store the tasks.

The for loop uses a nested loop to populate the text area. It checks to see if an hour property on a tasks object exists that matches each time slot and then sets the text of that box to the text property if it does.

Finally, the scheduler uses moment.js to display the current date to the user. It also uses m.hours and an array of military time integers to compare whether the timeblock it is rendering is in the past, present, or future, based on when the user logs in, and sets the styling accordingly.

Check it out at https://paulsloderbeck.github.io/dayscheduler/

![ScreenShot](https://github.com/paulsloderbeck/dayscheduler/blob/master/screenshot.png)
