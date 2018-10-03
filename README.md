# Adding Heart Rate Data to Strava TCX File

I changed phones and forgot to sync my heart rate monitor before heading out on a ride. While downloading the TCX file for the activity from Strava was easy, there was no easy way to edit it or to otherwiwise add heart rate data to an existing activity.

The notebook included here is a quick parsing of the TCX xml file that adds in heart rate data and then writes a new file.

That file can then be uploaded to Strava. Strava won't let you upload a duplicate activity (not sure how they determine duplicates, but it's more complicated than just changing the Lap Id and StartTime. The notebook has a switch for adding in a time delta so that you can upload the revised file to check it before deleting the original activity and uploading the revised file with the same time stamps as the original activity. **Note that you will lose all of the kudos and comments associated with your original activity when you delete it.**
