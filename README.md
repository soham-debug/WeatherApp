# WeatherApp
We need to login at openweathermap.org site then go to my profile and select my api keys and then generate the key after that go to API tab menu and click on API doc of current weather data then copy this https://api.openweathermap.org/data/2.5/weather?q={city name}&appid={API key}
and after that open postman create a new workspace and create a collection then paste this  https://api.openweathermap.org/data/2.5/weather?q={city name}&appid={API key} in get method in postman then 2 fields will be created and then we have to write the city name in q filed and paste our generated API key in the appid field after that click on send if you are trying for the first time then it will gives u an error because the generated API key need 1hour to get activated so we have to wait for 1hour only for the first time 
After this we have to open VS code and create a new project then go to tools and then nugets manager then we have to install cpprest 142 version after that we have to go to project section and then properties after that go to c/c++ -> general -> additional include we have to import include file of cpprest in it and then go to linker -> general and then additional libraries -> import cpprest lib file in it then we have to install vcpkg by using cmd following are the commands 

-git clone https://github.com/microsoft/vcpkg.git

-cd vcpkg

-./bootstrap-vcpkg.sh  # For Linux/macOS
.\bootstrap-vcpkg.bat  # For Windows

-.\vcpkg integrate install

-.\vcpkg install cpprest:x64-windows

After this we have to write the code then build the code then run it and 
our project is successfully completed :) 
