# TASK

Create a simple React application which displays the current wind and humidity
for Copenhagen provided by the OpenWeatherMap API.
To see your progress as you go, you may want to uncomment the render call in STEP 3 first!

[Codesandbox](https://codesandbox.io/s/green-flower-v13z0247?file=/src/index.jd)

### STEP 1:

Create a component to recieve data from the OpenWeatherMap "current weather" API.
OpenWeatherMap current DOCUMENTATION: https://openweathermap.org/current
It should:

1. Recieve data from the OpenWeatherMap apiUrl (defined below as `apiUrl`)
2. Store the recieved data in state with a time stamp the time the data was recieved
3. Pass the data and timestamp to it's children using the "children as a function" pattern.
4. Recieve new data from the OpenWeatherMap API every 3 seconds and update state appropriately

```
let apiKey = "";
let apiUrl =
"//api.openweathermap.org/data/2.5/weather?q=Copenhagen,dk&units=metric&appid=" +
apiKey;
```

### STEP 2:

Create a component which utilises your above component to display:

1. The current wind speed and direction
2. The current humidity percentage
3. The time when the data was last updated

### STEP 3:

Render the application here. I'll make this part easy :)

```
const rootElement = document.getElementById("root");
ReactDOM.render(<App />, rootElement);
```
