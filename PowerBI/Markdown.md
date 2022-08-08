# Whatsapp Dashboard for group chat

>This dashboard is based in the same dataset used in the Jupyter Notebooks: The exported whatsapp chats without including multimedia after being proccesed and cleaned. For this particular project I'm connecting to a MySQL database that contains all the information, which is updated by me weekly (Cleaning and Updating notebook in the root directory).

## What information does the dashboard contain?

The dashboard is separated in two different sorts of tabs: The "Main" tab and the "User" tab:

### Main tab

This tab contains global information regarding the group chat, and contains the following elements:

#### Group Members

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/GroupMember.png?raw=true)

This section contains various buttons with the alias of each group member, clicking on any of them allows us to check their User tab and review their group activity.


#### Messages Sent by User

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/AuthorsActivity.png?raw=true)

This bar chart shows how many total messages have been sent by each User. Each one is sorted downwards and using the scroll is possible to see the rest. Considering the numebr of aprticipants, a pie chart would've been innapropiate.


#### Messages sent each day of the week

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/MessagesPerDay.png?raw=true)

In this polar chart is possible appreciate the global group behaviour divided into each day of the week: It's curious that there is a considerable decrease of activity on weekends, opposed to a greater ammount of messages sent during working days.


#### Global overwiew of group activity by Date

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/MessagesPerDate.png?raw=true)

This line chart allow us to take a look at the group's complete behaviour from the date the first register was added into the database. There have been some highs and lows, but we're still going! :).

An important detail to consider regarding the decrease of activity at the end of the graph is that the database is updated each sunday afternoon, so messages for the last day of the update are consistently lower because the day isn´t over at that point.


#### Global overwiew of group activity by Time

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/MessagesPerTime.png?raw=true)

This chart answers the question: At which time of the day is the group at it's highest activity? It shows how the message flow behaves at different times of the day; unsurprisingly the highest peaks are around luch break and the end of the day (the darker areas in the chart)


#### Word Cloud

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/WordCloud.png?raw=true)

With the WordCloud we can see which are the most used words or expressions used globally, this includes emojis and interjections that may lose significance without proper context, but which are interesting to consider nevertheless.


#### Weekly Indicators

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/WeeklyIndicators.png?raw=true)

This indicators are updated each week (starting at mondays) and compares the group metrics with the previous week one's. The metrics to consider are the following:

**- Total Sent Messages:** The ammount of messages sent at the current week. In this case there was a 34.99% decrease compared to the previous week.

**- Average Daily Messages:** The average ammount of messages sent by day on the week. In this case there was a 8.99% decrease compared to the previous week.

**- Average number of words per message:** What is the average ammount of words contained in the week's messages. In this case, there was no increse or decrease in this metric. This one is rounded because there is no such thing as a half-word or 5.73 words, so it wouldn't make sense to present the value as such.


#### Total messages sent

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/Total.png?raw=true)

This indicator shows us the total ammount of messages that are stored on the database; over which the analysis is performed.


#### Date Filters

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/DateFilters.png?raw=true)

Let's say that we don't want to check the most recent data, but to check data from the last 3 weeks, or the last 2 days, or between June 3 and July 2. This is possible using either the simple filter (left) or the manual filter (right). This allows a full comprehension of the data in any time period as the user desires to review. 


#### Information

![](https://github.com/JhoaoAle/WhatsappDashboard/blob/main/PowerBI/Pictures/Markdown/Info.png?raw=true)

Clicking this button from the Dashboard will redirect the user to this Markdown file.
