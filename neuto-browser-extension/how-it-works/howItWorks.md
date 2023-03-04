## Neuto Browser Extension is an easy way to get an insight into your browsing activity. The extension measures every page you load in your browser and provides a rough estimate of the associated carbon emissions. We built this tool primarily to raise awareness about how browsing the web affects the world around us.

By [Alex McCartney](https://alexmccartney.com)

### What happens

Neuto Browser Extension runs a background script in your browser each time you navigate to, or load, a webpage. After it has performed its tasks, this script changes the colour of our icon to green or black, depending on the extent of the carbon emissions that the current webpage generates. This information is stored in your browser cache and is accessed when you click on our icon to view the specific number of grams of CO2e generated, alongside a tally of your total emissions during the current browsing session. We’ve also included a useful graphic to show how this webpage performs in comparison to an ‘optimised’ webpage.

### The calculations

For the Neuto Browser Extension, we utilise a set of constants agreed upon by multiple organisations using estimates for the following:

Annual Internet Energy: 1988 TWh

Annual End User Traffic: 2444 EB

Annual Internet Energy / Annual End User Traffic = 0.81 kWh/GB

Carbon Factor (global grid): 442 g/kWh

Though these are estimates, they enable us to get a rough idea of a website’s carbon emissions without requiring much data. In fact, the only data we then need to complete our calculation is the ‘page weight’ or ‘data sent down the wire’. This method therefore protects the privacy of users and website owners to a significant extent.

The final formula we use looks like this: 

Emissions = Energy(kWh) * Carbon Factor(g/kWh)

Emissions = (( data * 0.81 ) * 442 )

For the browser extension, we’ve had to make some additional assumptions. We are running the extension in a browser, which takes care of any caching amendments we might otherwise have to make. We’ve used only the ‘global grid’ Carbon Factor, as we don’t know what the mix of grid and renewable energy will be for any individual user. It would be possible to add this capability using data on country-specific energy mixes but it might raise privacy concerns if at some point we developed an external API to accompany the browser extension.
