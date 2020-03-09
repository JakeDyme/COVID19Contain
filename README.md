# COVID19Contain
To develop apps with the objective of containing the COVID-19 outbreak

<!-- wp:paragraph -->
<p><em>I'm writing this because I need help to develop a mobile app. Although I am a developer, I'm not a mobile-app developer and as much as I would like to use the opportunity to learn app development, I feel like getting this app out there as quickly as possible is worth more than my desire to upskill.</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Ok so COVID-19 AKA Corona Virus has gone viral. Its no joke, its spreading rapidly and everyday there seem to be new cases popping up everywhere in countries all around the world. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>By the time that you know that you're infected you've probably already infected others, and by the time they find out, they've infected others too. When people do eventually realize that they have it they try their best to quarantine themselves, but by then the damage is done, the virus is spread, and there are new unwitting hosts casually spreading it as they go about their daily dues. If only we could go back in time and tell everyone that we'd come into contact with to quarantine themselves. Well we would need a time machine for that, which obviously we don't have... or do we?</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>So here's the pitch. Imagine if everyone had an app on their phone that tracked their movement from place to place. Sound creepy? Well google is doing it already, if you're like me you can go see all the places you've been just by looking at your timeline in google maps. I'm not saying that we use that information (but if we can then lets do that). For now I'm going to assume that we can't use that info. So the COVID-19 App (or Capp for short) will track your movement between places once you've activated the app. Now here's where the magic starts, lets assume hypothetically, that everyone is using the app, and has had it activated for the last month. Someone in the network discovers they that they have the virus and they hit the red button on the app. The app then checks their movements for the last month (because so far the max incubation period recorded is 27 days). For all member's who's places intersect the infected persons places at the same point in time (+12hrs), those members can be notified that they are at risk and should self-quarantine. In a cascading fashion the app can also immediately determine from the point of intersection in time and place, who the newly infected members might have inadvertently infected after their own potential contamination, and can raise a secondary risk to all those additional members. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>That's the gist of it. Its not the simplest app but I'm pretty sure it can be done. Why do this? Well, if we don't get smarter about how to contain this thing now then we could either end up with a full blown global pandemic, or an economic collapse. This is option 3, and I think its a good one, but we need to work together. With enough participation we can keep our countries running while at the same time keep the high risk individuals quarantined until its safe.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Our objectives are simple: </strong><br>a) Build this app in the shortest amount of time.<br>b) Get everyone with a smart mobile device to use it.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Here are some Initial Technical Requirements:</strong><br>- The app needs a button for people to push if they discover that they have the virus.<br>- There needs to be a server to capture the data and push notifications out to devices.<br>- There must be a risk meter which will give people a risk-of-infection score based on factors.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Example Algorithm</strong><br>- [PersonZ] identifies as being infected. Risk level: [MAX] (by pressing the "Infected" button)<br>- Places visited by [PersonZ] in last 27 days are [Address:A] at [Time:N] on [Date:Today-10days]<br>- People who visited [Address:A] on [Date:Today-10days] from [Time:N] to [Time:N+12hrs] are [Person:X];<br>- [Person:X] is marked as being potentially infected. Risk level: [HIGH]<br>- Places visited by [PersonX] in last 10 days are [Address:B] at [Time:G] on [Date:Today-3days]<br>- People who visited [Address:B] on [Date:Today-3days] from [Time:G] to [Time:G+12hrs] are [PersonY]<br>- [Person:Y] is marked as being potentially infected. Risk level: [MED]<br>- Places visited by [PersonY] in last 3 days are [Address:C] at [Time:H] on [Date:Today-1days]<br>- People who visited [Address:C] on [Date:Today-1days] from [Time:H] to [Time:H+12hrs] are [<em>none</em>]</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Send MAX risk alert to [PersonX]</li><li>Send HIGH risk alert to [PersonY]</li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p><strong>Implementation details</strong><br>- Place tracking can be done on the client, and risk assessment could probably be done there too, or we could offload that into the cloud if compute is too high.</p>
<!-- /wp:paragraph -->
