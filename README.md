# candidate-emails

This repository contains the data behind the story [Which Democrats Are Campaigning On Trump?](https://fivethirtyeight.com/features/which-democrats-are-campaigning-on-trump).

We've subscribed to the email lists for every 2020 Democratic campaign that FiveThirtyEight [considered "major"](https://fivethirtyeight.com/features/heres-how-were-defining-a-major-presidential-candidate/) in the month before the first night of the first Democratic debate (June 26) using the ZIP code of FiveThirtyEight's New York City office, meaning we may not be getting the same amount — or type — of emails as some other subscribers because campaigns can target emails to specific groups of people. To protect our email address from spam, any reference to it has been replaced with `****@****.****`.

`emails/` contains an HTML file for every email we recieved organized into folders by the name of the candidate who sent it.

`index.csv` is an index of emails in the `emails/` folders along with the subject line of the email, the email address of the campaign, and the date on which it was received.

Column | Description
-------|---------------
`candidate` | Name of candidate
`message_id` | Unique identifier for each email
`message_date` | [Date and time](https://developers.google.com/gmail/api/v1/reference/users/messages#internalDate) at which the message was recieved
`message_from` | Sender, email's `From` header
`message_subject` | Subject, email's `Subject` header
`filepath` | Path of the file in this repository containing the HTML body of the email
`url` | Path of a URL where the HTML body of the email can be viewed online
