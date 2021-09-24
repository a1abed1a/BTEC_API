# Designing and Implementing an application that incorporates relevant APIs

## Investigate appropriate APIs

- [**locationiq**](https://locationiq.com/)  
   - Description:  
     LocationIQ offers enterprise-class, adaptable, location-based solutions. They collaborate with developers, entrepreneurs, and organizations around the world to serve billions of orders.

   - Usage:      
     - Static Maps  
       Requests can be sent to the following endpoint  
       GET `https://maps.locationiq.com/v3/staticmap`

   - Endpoints/Request URLs:  
     Depending on which Maps SDK you decide to use, you will need to use either the Style Specification URL or Tile URLs.

     Style Specification URL:

     For Mapbox-GL SDKs, use a Style Specification URL. A Style URL looks like this:

     `https://tiles.locationiq.com/v3/<theme>/<type>.json?key=<access_token>`

     Tile URLs:

     For LeafletJS and other mapping libraries, you need to specify Tile URLs instead:

     `https://{s}-tiles.locationiq.com/v3/<theme>/r/{z}/{x}/{y}.<format>?key=<access_token>`

   - Authentication Key:  
     To avoid misuse, create a different access key for each program, name it appropriately, and renew these keys on a regular basis. Access keys can be used in both public and private contexts.
     My key(pk.c501b86a237fbc1b1a613cb8a80954da)

- [**themoviedb**](https://www.themoviedb.org/)  
   - Description:  
      The Movie Database (TMDB) is a movie and tv database created by the community. TMDb's international emphasis and range of data are unrivaled. It is meant for people who want to use pictures and/or data from a film, television show, or actor in their application. The API is a mechanism that allows data and/or pictures to be retrieved and used programmatically.

   - Usage:  
       - Search Keyword 
         Requests can be sent to the following endpoint  
         GET `https://api.themoviedb.org/3/search/movie`

   - Endpoints/Request URLs:  
      Get movies by Keyword  
      `https://api.themoviedb.org/3/search/movie?api_key={api_key}&query={Keyword}`

   - Authentication Key:  
      To avoid misuse, create a different access key for each program, name it appropriately, and renew these keys on a regular basis. Access keys can be used in both public and private contexts.
      My key(f7a47b966bb41bd369d80c2272050bd4)

- [**weatherbit**](https://www.weatherbit.io/)  
   - Description:  
      It can access current weather observations, historical weather data going back more than a decade, Doppler radar, satellites, and atmospheric reanalysis products. In addition, extremely localized weather forecasts for every location on the planet are provided using the world's most accurate weather models.

   - Usage:  
       - 16 Day Weather Forecast  
         Requests can be sent to the following endpoint  
         GET `http://api.weatherbit.io/v2.0/forecast/daily`

   - Endpoints/Request URLs:  
       Get forecast by lat/lon  
       `http://api.weatherbit.io/v2.0/forecast/daily?lat={lat}&lon={lon}&key={KEY}`

   - Authentication Key:  
      To avoid misuse, create a different access key for each program, name it appropriately, and renew these keys on a regular basis. Access keys can be used in both public and private contexts.
      My key(8cb07f0f81e94b8285d9a7240151de60)

