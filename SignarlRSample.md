Notes and codes using SignalR building a CHATBOT
**
Some important notes:**
This example is based on the ASP.NET SignalR and not on the ASP.NET Core SignalR

Internet Explorer support
ASP.NET Core SignalR doesn't support Microsoft Internet Explorer, whereas ASP.NET SignalR supports Microsoft Internet Explorer 8 or later. For more information, see ASP.NET Core SignalR supported platforms.



What is SignalR?
ASP.NET Core SignalR is an open-source library that simplifies adding real-time web functionality to apps. Real-time web functionality enables server-side code to push content to clients instantly.


**References**
Video: https://www.linkedin.com/learning/learning-signalr-with-asp-dot-net-core/add-a-signalr-hub?resume=false&u=89213594
https://learn.microsoft.com/en-us/aspnet/core/signalr/introduction?view=aspnetcore-8.0

Good Candidates for SignalR:
* Apps that require high frequency updates from the server. Examples are gaming, social networks, voting, auction, maps and GPS apps.
* Dashboards and monitoring apps. Examples include company dashboards, instat sales updates, or travel alerts.
* Collaborative apps. Whiteboard apps and team meeting software are examplesof collaborative apps.
* Apps that require notifications. Social networks, email, chat, games, travel alerts, and many other apps use notifications.

SignalR uses hubs to communicate between clients and servers.
![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/69ba4692-a93a-4590-aac9-20d63de534a9)





IT'S IMPORTANT TO PLACE THE SIGNALR MIDDLEWARE AFTER HTTPS AND YOUR AUTHORIZATIONS SEE PICTURE BELOW
![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/a44fd709-f343-4943-8145-89177bbb513e)


NOTE: SIGNALR is usually ** implemented is to include them as part of your project(NUGET) not as CDN** 


Example code:
When loading your chatbox you can prompt the DISPLAY msg using the OnConnectedAsync
![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/a7ccf601-8f54-4ebc-b781-96210ba55692)



Codes that loops the chatbox to reconnect after 5secs after being disconnected 
![image](https://github.com/CryptoEmo-dev/.NetNotes/assets/123077155/55897d7f-681b-41b7-990b-41e1fcc15c89)










