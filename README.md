Add in the tutorial image here 

![Tool Logo](Image filename)

# Geocoding aka Address Matching
This tutorial provides step by step instructions for matching a table of addresses to a geographic database using ArcGIS technologies. This process is called "Geocoding". Geocoding consumes 'credits' in the Esri ecosystem. As a user at Brock University (or other 'organization' with a site license) you will be allocated a limited number of credits. Brock University affiliates should contact maplib@brocku.ca before attempting to geocode a table with greater than 100 records.

More details about credits can be found [here](https://www.esri.com/en-us/arcgis/products/credits/overview?rsource=%2Fsoftware%2Farcgis%2Farcgisonline%2Fcredits)  

----

## Setup Instructions
In preparation for this tutorial, you will need an organizational account. As a Brock University affiliate, you already have such an account. The first part of the tutorial will outline steps for accessing the software using your Brock credentials.  

NOTE: ArcGIS Pro is a Windows-based software and will NOT run on a Mac computer unless you have Parallels or Bootcamp installed. Contact Campus ITS in the Campus Bookstore for more information.  

NOTE: Brock University has a site license for ArcGIS Pro. Therefore, you may download and install the software on any Windows machines for academic and research purposes. ArcGIS Pro can be found on any PC across campus. The Map, Data & GIS Library also has a special Alienware PC for use by the Brock community.  

https://youtu.be/GqH4UHTUf2s  

Download the Excel file used in this tutorial. Niagara Sports Facilities [acquired from https://niagaraopendata.ca/dataset/niagara-sports-clubs-facilities](https://niagaraopendata.ca/dataset/niagara-sports-clubs-facilities) 

![image](https://user-images.githubusercontent.com/45638590/227005932-a60acb9f-3b34-4203-9088-5f012f652355.png)

OR...
The CSV is available [here](NiagaraSportsFacilities.csv).  

----

## Tutorial Steps

1. Run ArcGIS Pro.
2. Sign in using your Brock credentials as per [this video](https://youtu.be/GqH4UHTUf2s) (NOTE: download instructions are also included in the video)
3. New Project > Map ![image](https://user-images.githubusercontent.com/45638590/227007092-cd43a99b-9b42-4152-a8ca-44f35939986f.png)  

4. Create a new project ("Geocoding Tutorial") and define the working directory (local storage is recommended).  
 ![image](https://user-images.githubusercontent.com/45638590/227007255-e290f578-fdfb-4353-a90b-6c9803f4e25b.png)  
 
5. Click OK. The software generates a new map project with a project folder and geodatabase.
6. By default there is a basemap projected to **WGS 1984 Web Mercator (auxillary sphere)**.
7. Click the Map tab at the top and click the Add Data button. ![image](https://user-images.githubusercontent.com/45638590/227008015-26c10409-bc60-42d9-ae8e-cdc336f8519f.png)  
8. Browse to the download directory holding the NiagaraSportsFacilities.csv Select the file and click OK.
The table appears in the Contents pane under Standalone Tables:

![image](https://user-images.githubusercontent.com/45638590/227008580-a7c08919-b388-4492-9c60-3ec9ebc785f9.png)  

9. Right-click the table under Contents and click Open. Browse the available attributes and notice the address fields. We will match the addresses in the table with the Esri World Geocoder to plot points on the map.
10. Close the table.
11. Right-click the table under Contents and click Geocode Table.
![image](https://user-images.githubusercontent.com/45638590/227594718-e6fe8d94-7661-4e1f-ad61-d10eff85dc5b.png)  The Geocode Table wizard appears to the right of the map view. Navigate through the pages as follows.  
12. Page one outlines the steps involved. Click Start at the bottom of the page.  
13. Step One: from the **Input Locator** box, select **ArcGIS World Geocoding Service** ![image](https://user-images.githubusercontent.com/45638590/227595597-36186f55-7200-4d7c-881d-4f349f5f2063.png).  Click Next.

**NOTE: Geocoding consumes credits. Please contact maplib@brocku.ca before attempting to geocode a table with over 500 records.**

14. Step Two: This page prompts you to identify how your data is structured. This particular table has the addresses stored in more than one field. Accept the default and click Next.  
15. In Step Three, the software attempts to match fields in the CSV with known fields in the address locator. Accept the defaults and click Next.  

![image](https://user-images.githubusercontent.com/45638590/227596541-53cc754f-600d-468c-893f-f85c14e88556.png)

16. For Step Four: Output, you can define where the resulting feature layer is created. Accept the defaults for now and click next.  
17. For Step Five: Select Canada. This helps the software know the location more accurately. Click Next.    
18. For Step Six: Select the categories Address and Postal ![image](https://user-images.githubusercontent.com/45638590/227597232-6337b58a-fc04-4211-a982-95e1eaaf12eb.png).  Click Finish.  
19. From the summary page, notice the option at the top to calculate an estimate of how many credits will be consumed. Users at Brock University will have 300-500 credits by default. This activity will consume 9.08 credits.  
20. At the bottom of the page, click Run.  
21. When the process is finished, you will see a **Geocoding Complete** window. Here you will have the option to rematch any unmatched records. Click No.

![image](https://user-images.githubusercontent.com/45638590/227598587-38122e37-7632-4f78-96a7-a34d9aab67f6.png)  

The map now shows points representing sports facilities in the Niagara Region and you will see a new feature layer in the Contents pane on the left.  

![image](https://user-images.githubusercontent.com/45638590/227598970-e3f10177-21e4-44fe-ac40-f0077e1fc513.png)




----

## Next Steps (Optional)
This is where you can add any additional resources, follow up tutorial, or workshop reccomendations that users might use to continue learning about the tool described in the tutorial.  The more the better!

----

**This tutorial is supported by the Brock University Research Lifecycle Department; Map, Data & GIS Library.  If you have any questions or concerns regarding this tutorial, don't hesitate to contact [maplib@Brocku.ca](mailto:maplib@Brocku.ca)**
