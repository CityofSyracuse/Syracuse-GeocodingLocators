### Syracuse Geocoding Locators

This Locator file allows you to do unlimited Geocoding (adding Latitude & Longitude Coordinates) on your local machine, without paying $$$ to ESRI or Google API for this.

### To use:

To be able to use a locator file, you need to hae ArcGIS Pro on your computer.  If you are a member of the ArcGIS pro to use.

1.  In ArcGIS Pro, go to the **Map** tab up top, then add the address data that you would like to obtain Latitude & Longitude information on (most likely a table dataset).
2.  Download the locators files in this repository.
3.  Add the Locator files to your project.  To do that go to the **Insert** tab up top, then click **Connections**, then **Add Locator**.
4.  You will then navigate to where the downloaded locators are, then press **OK** to add this Locator to your **Project**.
5.  Then in the **Conents Pane**, right lick on your Datatable that you want to get Latitude and Longitude information on, and select **Geocode Table**.
6.  This then takes you through the Geocode Wizard, where you will select which Input Locator you are using.  (We have found SyrStreets to work beds for the 100 Block Level crime data), and the **SyrPoints_Streets_CompositeAdd** to work best for most other addresses.
7.  You then select if the address is in more than one field or more than one field.
8.  Then select the name of the column that containes the address values ("Address" in the Crimes files).  
9.  I have been keeping the selection of (add output to map after completion, Address Location, and Output Fields "All" selected.
10. I have also been keeping the Category section unchecked (If you only wanted to match to address, and not intersection, or stret name, you can select only the ones you want to include.  I have kept all, because often Crime addresses may be in the form of an intersection and not a traditional address.)
11. Then click finish, and make sure that your **Output** Name does not include any special characters, such as a $ (because this will throw an error).  If it does have any special characters, just click the Folder Icon and delete the special characters.
12. Then 
### TO DO.

1. Work on a Python Script to Automatically Run this in ArcGIS Pro after the Crime Data has been updated, to automatically Geocode the New Crime files and replace the info in the 2022 Crime Data Part 1 with Lat & Long with this new Geocoded dataset.
