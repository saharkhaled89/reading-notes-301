# What Google Learned From Its Quest to Build the Perfect Team

**Project Aristotle’s researchers began by reviewing a half-century of academic studies looking at how teams worked. Were the best teams made up of people with similar interests? Or did it matter more whether everyone was motivated by the same kinds of rewards? Based on those studies, the researchers scrutinized the composition of groups inside Google: How often did teammates socialize outside the office? Did they have the same hobbies? Were their educational backgrounds similar? Was it better for all teammates to be outgoing or for all of them to be shy? They drew diagrams showing which teams had overlapping memberships and which groups had exceeded their departments’ goals. They studied how long teams stuck together and if gender balance seemed to have an impact on a team’s success.**


# Which group would you rather join?

**As the researchers studied the groups, however, they noticed two behaviors that all the good teams generally shared. First, on the good teams, members spoke in roughly the same proportion, a phenomenon the researchers referred to as ‘‘equality in distribution of conversational turn-taking.’’ On some teams, everyone spoke during each task; on others, leadership shifted among teammates from assignment to assignment. But in each case, by the end of the day, everyone had spoken roughly the same amount. ‘‘As long as everyone got a chance to talk, the team did well,’’ Woolley said. ‘‘But if only one person or a small group spoke all the time, the collective intelligence declined.’’**



**How I explained REST to my brother**

* using verbs and nouns while writing programs

* show the concepts with realistic examples.

# SuperAgent

**SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!**

**Test documentation**

**The following test documentation was generated with Mocha's "doc" reporter, and directly reflects the test suite. This provides an additional source of documentation.**

# Parsing response bodies

**SuperAgent will parse known response-body data for you, currently supporting application/x-www-form-urlencoded, application/json, and multipart/form-data.**

# JSON / Urlencoded

**The property res.body is the parsed object, for example if a request responded with the JSON string '{"user":{"name":"tobi"}}', res.body.user.name would be "tobi". Likewise the x-www-form-urlencoded value of "user[name]=tobi" would yield the same result. Only one level of nesting is supported. If you need more complex data, send JSON instead.**

**Arrays are sent by repeating the key. .send({color: ['red','blue']}) sends color=red&color=blue. If you want the array keys to contain [] in their name, you must add it yourself, as SuperAgent doesn't add it automatically.**

# Response properties

**Many helpful flags and properties are set on the Response object, ranging from the response text, parsed response body, header fields, status flags and more.**

## Response text

**The res.text property contains the unparsed response body string.**

## Response body

**Much like SuperAgent can auto-serialize request data, it can also automatically parse it. When a parser is defined for the Content-Type, it is parsed, which by default includes "application/json" and "application/x-www-form-urlencoded". The parsed object is then available via res.body.**

## Response header fields

**The res.header contains an object of parsed header fields, lowercasing field names much like node does. For example res.header['content-length'].**

## Response Content-Type

**The Content-Type response header is special-cased, providing res.type, which is void of the charset (if any). For example the Content-Type of "text/html; charset=utf8" will provide "text/html" as res.type, and the res.charset property would then contain "utf8".**

## Response status

**The response status flags help determine if the request was a success, among other useful information, making SuperAgent ideal for interacting with RESTful web services.**


# Weather API Call Types

## We provide two types of API requests to retrieve the weather anywhere in the world:

* The Forecast Request returns the current weather forecast for the next week.

* The Time Machine Request returns the observed or forecast weather conditions for a date in the past or future.

* Weather Conditions

## The Dark Sky API offers a full collection of meteorological conditions in 39 different languages, including:

* Apparent (feels-like) temperature

* Atmospheric pressure

* Cloud cover

* Dew point

* Humidity

* Liquid precipitation rate

*Both forecast and time machine requests return the same weather conditions, in the same convenient JSON format. You can parse the response directly, or use one several community-contributed libraries to interact with our API in the programming language of your choice.*


