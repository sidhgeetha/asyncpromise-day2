## Design app and show Restcountries and weather using fetch API ##

   1. JS code -> get the URL link URL = "https://restcountries.com/v3.1/all"; to to fetch data about rest countries.
   2. create new instance of XMLHttpRequest and store it in XHR object.
   3. It opens a GET request to the specified URL using xhr.open() and sends the request using xhr.send()
   4. Added event listeners xhr.onreadystatechange = () => {} to track changes in the state of an (XHR) object. this event happend whenever the ready state is changes.
   5. Added event listerner    xhr.onprogress = () => {} to indigates the data being loaded.
   6. xhr.onload = () => {} tells that data is completely loaded in xhr.response wwhich is JSON format. used const result_array = JSON.parse(xhr.response); to convert JSON data into javascipt object.
   7. Used for loop to iterate the each data in result array.
   8. Called the function names createCard() with arguments for the properties given in fundtion create card as obj.flags.png, obj.name.common, obj.capital, obj.region,obj.cioc, obj.latlng[0], obj.latlng[1].
   9. Inside the function createCard , created DOM element as column "div" stored in varibale column. Added classlist "col-lg-4", "col-sm-12" from bootstrap.
      1. Created DOM element for card with class name card card-header card-body text-center"
      2. Created DOM element for img,
      3. Created DOM element for cardhead as "div" stored in cardHead
      4. Created DOM element for cardbody as "div" stored in cardBody
      5. Created DOM element for cardTitle as "h5" stored in cardTitle.
      6. Created DOM element for capitalName as "p" stored in capitalName
      7. Created DOM element for regionName as "p" stored in regionName
      8. Created DOM element for cioc as "p" stored in cioc
      9. Created DOM element for  lat/log as "p" stored in lat and log
      10.  Created DOM element for button as "button" stored in cardLink with the class name "btn btn-primary "
      11.  And gave innerHTML value for button as "Click for Weather";
      12.  added click event for cardlink button and
      13.  Had a arrow function when the fucntion is clicked and called get weather function with arguments lat and log to have weather data.
      14.  Than appends the card element  to the column element. card to show country inromation.
      15.  Created DOM element "row" adn appends the column inside row lements that is  add cards into row.
     
  10. at last, opened function named getweather with properties lat and log
  11. Used URL for the API request using the latitude and longitude.
  12. Fectched data using response.JSON as JSON data
  13. next then() block is to log data.
  14. applied necessary CSS for for DOM elements img.style , cardHead.style, cardBody.style, ..
    
          

       
   
   
