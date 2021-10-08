Here is a brief description of each file.

File "states.txt":

contains the possible states of the simulated user, as reported in the dataset file. 


File "entertainment.txt":

contains the locations of 1280 entertainment places and a rating value for each place. The file is in CSV-like format, with ':' being the character that separates the columns. The locations and rating values have been crawled from the web. Places with higher rating values have higher probability to be chosen by users.


File "homes.txt":

contains the location of 30000 available houses. The file is in CSV-like format, with ':' being the character that separates the columns. At the beginning of simulation, users are uniformly distributed in these locations.


File "dataset.txt":

locations are stored in geographical coordinates. The file is in CSV-like format, with '_' being the character that separates the columns. To save space, samples in which the property of a user are unchanged are suppressed (e.g. if a user is located at the same place at two subsequent instants 10 and 11 and the activity state of the user is unchanged, the sample at instant 11 is not reported). Brief description of each column:


| id:		the ID of the user
| timestamp: 	absolute date and time of the sample
| longitude:    geographic longitude
| latitude:     geographic latitude
| frame:	relative time instant 
| checkin:      whether the user is issuing a check-in at the reported location (boolean value)
| actstate:	activity of the user (see "states.txt") 
| simstate:	movement state ("MOVING" or "STOPPED")

