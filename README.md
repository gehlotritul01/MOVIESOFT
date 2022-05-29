## Moviesoft App

This is my Microsoft Engage '2022 mentorship program webapp.
I have took challenge 3rd as my problem statement.

TOC
ReactiveSearch: Intro
Features
Component Playground
Live Examples
Comparison with Other Projects



1. ReactiveSearch: Intro
ReactiveSearch is an Elasticsearch UI components library for React and React Native. It has 25+ components consisting of Lists, Ranges, Search UIs, Result displays and a way to bring any existing UI component into the library.

The library is conceptually divided into two parts:

Sensor components and
Actuator components.
Each sensor component is built for applying a specific filter on the data. For example:

A SingleList sensor component applies an exact match filter based on the selected item.
A RangeSlider component applies a numeric range query based on the values selected from the UI.
A DataSearch component applies a suggestions and search query based on the search term typed by the user.
Sensor components can be configured to create a combined query context and render the matching results via an actuator component.

ReactiveSearch primarily comes with two actuators: ResultCard and ResultList. ResultCard displays the results in a card interface whereas ResultList displays them in a list. Both provide built-in support for pagination and infinite scroll views. Besides these, the library also provides low level actuators (ReactiveComponent and ReactiveList) to render in a more customized fashion.


2. Features
Design
The sensor / actuator design pattern allows creating complex UIs where any number of sensors can be chained together to reactively update an actuator (or even multiple actuators).
The library handles the transformation of the UI interactions into database queries. You only need to include the components and associate each with a DB field.
Built in live updates - Actuators can be set to update results even when the underlying data changes in the DB.
Comes with scoped and styled components. Doesn't require any external CSS library import, comes with className and innerClass support.
Is themable via ThemeProvider.
Ease of Use
One step installation with npm i @appbaseio/reactivesearch,
A UMD build that works directly in the browser. Installation steps here,
Styled and scoped components that can be easily extended,
See the reactivesearch starter app.
🆕 ReactiveSearch API: Secure your ElasticSearch Queries
Based on a popular request, we have implemented support for a declarative API based on ReactiveSearch. The API is called ReactiveSearch API. It moves the query DSL generation logic to a backend system (an appbase.io service) instead of exposing it directly on the client-side. By strictly enabling only ReactiveSearch API use, you can also prevent script injections.

The main advantages of using it over the ElasticSearch Query DSL are:

Query generation happens on the server-side - addressing the primary security concern around query injection.
Easy recording of analytics events for search and clicks. Read more
Application of query rules and functions for search queries. Read more
Using ReactiveSearch API instead of ElasticSearch's query DSL is an opt-in feature. You need to set the enableAppbase prop as true in your ReactiveBase component. This assumes that you are using appbase.io for your backend.

I recommend checking out this KitchenSink App that demonstrates the use of the ReactiveSearch API for all the ReactiveSearch components.



3. Component Playground
Try the live component playground at playground. Look out for the knobs section in the playground part of the stories to tweak each prop and see the effects.



4. Comparison with Other Projects
Here, i share how ReactiveSearch compares with other projects that have similar aims.

#	ReactiveSearch	SearchKit	InstantSearch
Backend	Any Elasticsearch index hosted on any Elasticsearch cluster.	Any Elasticsearch index hosted on any Elasticsearch cluster.	Custom-built for Algolia, a proprietary search engine.
Development	Actively developed and maintained.	Active issue responses, some development and maintenance.	Actively developed and maintained.
Onboarding Experience	Starter apps, Live interactive tutorial, getting started guide, component playground, every component has a live working demo with codesandbox.	Getting started tutorial, no live component demos, sparse reference spec for many components.	Starter apps, getting started guide, component playground.
Styling Support	Styled and scoped components. No external CSS import required. Rich theming supported as React props.	CSS based styles with BEM, not scoped to components. Theming supported with SCSS.	CSS based styles, requires external style import. Theming supported by manipulating CSS.
Types of Components	Lists, Ranges, Search, Dates, Maps, Result Displays. Can use your own UI components.	Lists, Ranges, Search*, Result*. Can't use your own UI components. (Only one component for Search and Result, resulting in more code to be written for customizability)	Lists, Range, Search, Result. Can use your own UI components.

5.You can run it on local host (http://localhost:3000/)


<img width="1440" alt="Screenshot 2022-05-29 at 4 26 41 PM" src="https://user-images.githubusercontent.com/88274354/170864477-46d6908b-e2df-4ebf-9506-d3c6f9aad915.png">

I have build this movie finder according to our moods web application using :- 
-Reactjs
-HTML
-CSS
-javascript
-Elastic Search : elasticsearch is a super-fast, open-source, full-text search engine. It                    allows you to store, search, and analyze big volumes of data quickly.            
-React search UI: to add searchbox,rating slider and filter components.
-Open Source React Search:open-source library to build this moviesoft webapp

Used Kaggle.com dataset for the movies
Logo :![logo](https://user-images.githubusercontent.com/88274354/170864747-ea75cb18-f6f7-4157-81f4-9ecb0387fc09.jpg) using Canva.



Instructions to run on your machine: (tip :p)

Since it is a react app when you will clone the repository make sure to run first remove all the json.lock ,yarn.lock and nodemodules if present and then re install it using 
"npm install".

After the installation is done give "npm start" command on your terminal and the app will start in the local host :).



Thank you so much :)

