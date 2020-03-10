# COVID19Contain
The development of apps with the objective of containing the COVID-19 outbreak

The purpose of this app is to be an early warning system to people who may be infected but who are not yet showing signs.
This is the most infectious time for the virus as people are unaware. With an early warning system people can opt in to self-quarantine in a bid to reduce the contagion.

Once activated the app tracks the places you visit, and when someone in the network identifies as being infected, everyone they have been in close proximity to gets a notification that they are potentially at risk of being infected. At that point people can choose to quarantine themselves or seek medical advise.

<!-- wp:paragraph -->
<p><strong>Initial Technical Requirements:</strong><br>- The app needs a button for people to push if they discover that they have the virus.<br>- There needs to be a server to capture the data and push notifications out to devices.<br>- There must be a risk meter which will give people a risk-of-infection score based on factors.</p>
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


<!-- wp:paragraph -->
<p><strong>Initial Technical Requirements:</strong><br>- The app needs a button for people to push if they discover that they have the virus.<br>- There needs to be a server to capture the data and push notifications out to devices.<br>- There must be a risk meter which will give people a risk-of-infection score based on factors.</p>
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
