# About

This is a simple COVID-19 tracking page for school districts. The data is pulled from a Google Sheet.

This is a modified version of [school-covid-tracker](https://github.com/korylprince/school-covid-tracker) that tracks Exposed and Symptomatic students and staff separately.

## Example

![Example Screenshot](https://raw.githubusercontent.com/korylprince/school-covid-tracker-split/master/screenshot.png)

# Setup

* Make sure <https://cdn.jsdelivr.net> is unblocked in your filter/firewall 
* Upload [template.ods](https://raw.githubusercontent.com/korylprince/school-covid-tracker-split/master/template.ods) to Google Sheets and convert it to a Google Sheet
* Edit the Campus names and counts on the Data Sheet
* Edit the student and staff count and As of Date on the Aggregation Sheet
* Share the Google Sheet to "Anyone on the internet with this link can view"
* Copy the ID from the Google Sheets URL.
  * **Example (ID is bold)**: <pre>https&#58;//docs.google.com/spreadsheets/d/<strong>1XYU0Q465AHurLjFKqjjLH8OsN8-WDERJP5wV3xZMilg</strong>/edit#gid=0</pre>
* Insert ID and District Name into the template URL: <pre>https&#58;//korylprince.github.io/school-covid-tracker-split/?district=<strong>{district name}</strong>&id=<strong>{id}</strong></pre>
  * **Example**: <https://korylprince.github.io/school-covid-tracker-split/?district=Example%20District&id=1XYU0Q465AHurLjFKqjjLH8OsN8-WDERJP5wV3xZMilg>
  * **Note**: Use `%20` in place of spaces in the District Name
* Add link to your website, or embed the page on your website (see below)

## Example Embed code

Replace `{district name}` and `{id}` using the instructions above. Adjust the width and height as necessary for your website.

```html
<div id="covid-wrapper" style="width: 100%; height: 100%; overflow: scroll;">

<iframe src="https://korylprince.github.io/school-covid-tracker-split/?district={district name}&id={id}" style="border: none; width: 710px; height: 1375px;"></iframe>
</div>
<div>If you have issues viewing the tracker, <a href="https://korylprince.github.io/school-covid-tracker-split/?district={district name}&id={id}">click here</a>.</div>
```

# Uses

* [Chart.js](https://www.chartjs.org/)
* [Material Design Icons](https://materialdesignicons.com/)
