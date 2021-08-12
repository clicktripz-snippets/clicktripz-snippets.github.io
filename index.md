# FlightHub Interstitial Testing
## Links
* <a href="http://staging17.justfly.com/">JustFly Staging URL</a>
* <a href="http://staging17.flighthub.com/">FlightHub Staging URL</a>

## Instructions
The interstitial ad will appear when the user leaves your site via the back button.

1. Ensure that the test domain has both the script tag and the `Interstitial` product enabled (via the Tower Dashboard).
2. Clicking a link above, transition to the test domain.
3. Ensure that a UCO is available on the site. If there isn't one, here's a minimal one that can be injected via the console.

```
window._CTZ = {
  enabled: true,
  "verticals": {
    "hotel": {
      "active": true,
      "search": {
        "city": "New York",
        "countryCode": "US"
      }
    }
  }
}
```
4. Click the back button to trigger the interstitial ad.

## Note
- If you're using a Chrome browser, please interact with the page before trying to trigger the unit.
