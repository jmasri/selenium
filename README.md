# Table of contents
1. [Login](##1.Login)
2. [Settings …(Feature under development)]
3. [Dashboard](##2.Dashboard)


# Torkin - Operator User Manual



Login

Settings …(Feature under development)

Dashboard

Providers

White List Updater Statuses

Export tab ( Info missing)

Tasks

Tasks Columns

Tasks Filters

Edit mode

Requirements

























## ##1.Login

To login to Torkin open the link: [https://torkin.goeuro.com.qa.goeuro.ninja/login](https://torkin.goeuro.com.qa.goeuro.ninja/login)

And enter your credentials:

--image here

For any problems with signing in, click on &quot; **Contact us**&quot;.



After signing in you will be navigated to the Torkin homepage, onto **&quot;Dashboard&quot;** page. In the Header, the user can configure the preferable language and their settings.

--image here

- Settings …(Feature under development)

Also, there is a possibility to log out.






## ##2.Dashboard

--image here

In this tab, the user can see the number of open tasks, Stations which were automatically created and the number of managed providers. Also in a table below the numbers present the data from the last run for the managed providers.

**Columns are split different categories:**

_Name_ (name of the provider)

_Mode_ (what kind of transportation the provider offers)

_Open_ (how many stations need to be done manually)

_Ready_ (how many stations were done automatically)

_Last run_ (timestamp of the last run of WLU for the provider).

The system gives the user the ability to view the opened and the ready tasks by clicking on the hyperlinked numbers.





1.
##
## 3.
Providers

In this tab, the user can manage the providers - to start the WLU (Wite list updater), rebuild the XML, change requirements, etc.

--image here

The user should see in the table the providers which are enabled from the operator&#39;s manager. The user can click on the play button to start the pipeline process for any provider in the list. Immediately after that, a new window will pop up, where the user has to select the requirements for the provider to run.

--image here

White List Updater Statuses

 When running the wite list update, the following statuses are expected to appear:

Once run, it will start with In Progress

--image here

Once the WLU finishes the status will change to Success

--image here

If WLU is not able to run for the provider then the status will be Failed

--image here

In this case, **please contact the admin**.

After finishing the WLU with status &quot;success&quot;, your tasks will be uploaded in tab &quot;Tasks&quot; and all the data for this provider will be overwritten (all the stations which are not done and merged) in Torkin.

1.
##
## 4.
 Export tab ( Info missing)









1.
##
## 5.
 Tasks

This tab is the main tab for updating the data for the provider&#39;s stations.

--image here

In this table, the user can see the tasks assigned to them.

Tasks Columns

The **station** column,  shows the name of the station according to the provider info, until the operator doesn&#39;t change the name. The in this field will be written the new name.

Next column is for the **provider&#39;s name**. the **Station type** shows provider type (bus or train or ferry).

**Coordinates** column shows the coordinates received from the provider in **red** until the user updates them. After the user&#39;s updates, the coordinates will be showing in **green**.

According to the requirements for the specific provider, there will be additional languages to be added as translations. All this can be seen in the **translation** column.

The last title in the table is for the **status** of the task. It could be &quot;open&quot; - if it is not started yet, or &quot;missing req.&quot; - if it is started but in progress.

Tasks Filters

On the top of the window, user can use filter fields. There the user can filter the results by status, coordinates, and provider. The status could be open and missing req. As mentioned earlier.

The coordinates can be Inaccurate which means they have to be adjusted and we still didn&#39;t start reviewing them. Another option for the coordinates is Missing. Sometimes the providers submit stations without coordinates. In this case, these tasks can be filtered with this field. The last option is Verified coordinates. This means that the coordinates were already adjusted.

With a click on the button  --image here , the user can start to edit the data for the related station.

Edit mode

This mode is designed to provide an easy and intuitive possibility to the user to enter the best data for the new position(station). Here the user can see where exactly is the position(station) on the map and to find if there are any suitable suggestions for this position/station

--image here

In Edit mode the window is divided into two parts. The left side is the map with the positions pinned on it. There the user can visualize the data on the map, with a blue pin marking the station that we have to import and green pins marking the suggested stations (stations from DB and Google which are close to the coordinates of the new station).

--image here

The user can choose a map to work with (Google Maps, OpenStreetMap, Yandex Maps or Tianditu).  For different countries the coverage of the map providers is different.

--image here

On the top of the left part, there is an option to check what is the original info for the station according to the provider.

On the right side is the window with a roadmap of the process, two tabs: for choosing an already existing position or for creating a new one, and the data (names, coordinates, providers).

--image here



The first step is to choose the coordinates for our new position. This could be done in two ways.

- &quot; **Choose from existing**&quot; -  if we have already a position in the DB which has good enough data to be used. Then the user can mark the position that match best our new station, clicking on the pin on the map and clicking on &quot;Select this position&quot; or clicking on the position from the list and again &quot;Select this position&quot; from the map.
- &quot; **Create new**&quot; - when the user can&#39;t find any suitable position and wants to create a brand new one. Here the coordinates could be manually entered



--image here

Or also the blue pin could be moved with drag-drop to the desirable place on the map and then the coordinates can be automatically prefilled clicking on the button &quot; **Prefill coordinates**&quot;.

--image here

When we have the coordinates the next step is clicking on the button &quot;Next&quot; which will guide us to the second part of the editing flow - &quot; **Add translation for this station**&quot;

--image here

Station names should be written in a way it&#39;s understandable in other languages and how they are used in other languages.

For example:

**Berlin hbf** translates to **Berlino hbf** in Italian.

The next step in &quot;Edit flow&quot; is editing the location(town).

The user can choose from the suggested locations:

--image here

By clicking on the pin on the map or choosing it from the list.

If the location is not represented on the map/ on the list then the user can create a new one using the tab &quot;create new&quot;

--image here

In the blank fields, the operator has to write the data which is necessary. (we will try to fill it in automatically but it is not implemented yet). The coordinates could be prefilled from the pin on the map with clicking on the button &quot;Prefill coordinate&quot; or they also can be manually written in the blank field. All the fields should be fill in. Once this is done then all the data can be saved with a click on &quot;Save&quot;

For the operator automatically will be open the next task from the list and the saved one will be moved to tab &quot;Export&quot; where can be deployed to the DB.

1.
##
## 6.
Requirements

This tab helps user in creating new tasks for required translations for new providers.

Once the stations for a provider have been entered, user can check the tasks list and update the stations marked in **Red**.

Once in update process, here the required translation field will appear with the selected languages required on this screen.

--image here

Editing requirements does the same function as adding, and can be reached using this button --image here

1.
##
## 7.
User Management
