## d3.chart boilerplate

Use this template to start your d3.chart contributions. A few guidelines:

1. You will need to use grunt > 0.4 to build your chart distribution files.
2. Run `npm install` to obtain the appropriate grunt tasks. Do not check in the `node_modules` folder - it is listed in the `.gitignore` file.
3. Replace the 'boilerplate' string (in its various capitalization throughout the project with the name of your chart.)

### Notes:

* You must use the name d3.chart-contrib-yourChart for your git repo name. We will be automatically searching for charts in that format and unless you specify them in this way, we won't find it.

* You must maintain your `package.json` with the appropriate versioning and dependencies.

* You must license your charts under the MIT Expat license or any other BSD-style license. 

* You must make sure your code passes linting. Proper code formatting please =).

* You should provide an example using the example folder structure. 

* You must not check in the files in the `dist` directory. When you are ready to release a version of your chart, run `grunt release` which will place builds into your root. Check only those builds in.

#### In the README: 

* You must clearly define what API your chart exposes - this includes getters/setters and any other methods that are available on the chart instance. Please refer to the recommended format on the d3.chart api page (TODO link to the API page)

* You must clearly state what events your chart is broadcasting and what arguments will be passed to the callbacks.

* You must provide sample usage of your chart type.

### API

Sample API Documentation:

#### `<instance>.highlight(value)`

**Description:**

Allows the highlighting of a specific value

**Parameters:**

* `value` - The value to highlight.

**Uses:**

Example:

```javascript
var chart = d3.select("#vis")
  .append("svg")
  .chart("Boilerplate")
  .higlight(12);
```

### Events

Sample Event Documentation:

#### `brush`

**Description:**

Broadcast when a circle on the chart is being mousedover

**Arguments:**

* `value` - The value corresponding to the circle being mousedover.

**Uses:**

Example:

```javascript
var chart = d3.select("#vis")
  .append("svg")
  .chart("Boilerplate");

chart.on("brush", function(value) {
  // handle event...
});
```

### Sample Use

Please provide sample use of your chart here.

## Contribution Statement

The ecosystem of d3.chart types will depend on the dilligence and hard work of people like you. By contributing a chart, you are growing our community and the value of d3. It does mean that you take responsability for your work. Please only contribute code that you feel is ready for others to use and do your best to maintain it as the d3.chart library evolves.

Thank you!