## MMR Vaccinations

This application was originally developed for the Chicago Department of Public Health (CDPH) to help Chicago residents identify a convenient no cost CDPH flu shot event. This version of the Vaccinate web application was created to help CDPH address a 2019 measles outbreak.

[https://measlesvax.chicago.gov/](https://measlesvax.chicago.gov/)

### BACKGROUND
In mid-2012, I went to a weekly meeting of civic coders where several city agencies presented. They asked for our help in building interesting applications around their available data. I was interested in the free flu shot clinic locations since flu season was coming up fast, and I had attended a free flu shot event in the past.

I built a prototype application and advertised it via Twitter. The Chicago Department of Public Health (CDPH), the Mayor's Office, and a few other civic coders, mainly Juan-Pablo Velez, noticed the tweet. Before I knew it, Juan-Pablo brokered a meeting between CDPH, the Mayor's Office, and ourselves. The meeting was positive and I began in ernest to polish up the application.

### BITS AND BYTES
Vaccination data used in this web application are published by the City of Chicago in their data portal at [https://data.cityofchicago.org/](https://data.cityofchicago.org/).
Vaccination events data could also be published as a Google Sheet. This code uses the Google Sheets API to retrieve event data. This application uses Google Sheets because it is easy to instantly update. Using a Google Sheet also makes this code more usable by agencies that have little to no technology resources.

#### Google Sheet Example:
[https://docs.google.com/spreadsheets/d/1_HTPvKSlLnWP__Lq_r-mCYKGcLau4Z7MmlsSyCMc454/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1_HTPvKSlLnWP__Lq_r-mCYKGcLau4Z7MmlsSyCMc454/edit?usp=sharing)

### MADD PROPZ
This web application could not have been originally built or executed without the sage feedback and assistance of Juan-Pablo Velez and Derek Eder. **Raed Mansour** (of CDPH) has been my advocate and full partner on the inside. Without his advocacy, this fairly unique relationship and this application would not work.

### CODE NOTES
This a HTML/CSS/JavaScript web application.

If you want to reuse this code for your city/county/province/state, a good place to start is in htdocs/js/config.json and htdocs/css/index.css and altering the properties. Anyone altering these files will need to be a little familiar with JSON ([https://www.youtube.com/watch?v=40aKlrL-2V8](https://www.youtube.com/watch?v=40aKlrL-2V8)) and CSS ([https://www.youtube.com/watch?v=6d_4sd_l7rQ](https://www.youtube.com/watch?v=6d_4sd_l7rQ))

If you want to change the javascript code I wrote, you'll find that in /src/js/index.js. I use Grunt ([https://gruntjs.com/](https://gruntjs.com/)) to minify and concatenate this file along with /src/js/ical.js ([https://github.com/nwcell/ics.js](https://github.com/nwcell/ics.js)) and /src/js/moment.js ([https://momentjs.com/](https://momentjs.com/)) I try to use meaningful variable names, so hopefully the code won't be too hard to follow.

### CODE REPOSITORY NOTES
I have been exceptionally terrible at organizing the code repository for Vaccinate and it has not gotten proper love over the last few years. I plan on changing my ways.

### ERRATA
This code should be fairly easy to take and use by other government agencies offering vaccine clinic events. If you would like any advice on implementing this code, drop me a line.

Tom Kompare
e: [tom@kompare.us](mailto:tom@kompare.us)
t: [@tomkompare](//twitter.com/tomkompare)