![ArcGIS Geocoding logo](world-geocoder-for-arcgis-220.png)

# Geocoding (Address Matching)
This tutorial provides step by step instructions for matching a table of addresses to a geographic database using ArcGIS technologies. This process is called "Geocoding". Geocoding consumes 'credits' in the Esri ecosystem. As a user at Brock University (or other 'organization' with a site license) you will be allocated a limited number of credits. Brock University affiliates should contact [maplib@brocku.ca](maplib@brocku.ca) before attempting to geocode a table with more than 1000 records.

More details about credits can be found [here](https://www.esri.com/en-us/arcgis/products/credits/overview?rsource=%2Fsoftware%2Farcgis%2Farcgisonline%2Fcredits).  

----

## Setup Instructions
In preparation for this tutorial, you will need an organizational account. As a Brock University affiliate, you already have such an account. The first part of the tutorial will outline steps for accessing the software using your Brock credentials. [Video instructions](https://youtu.be/GqH4UHTUf2s). 

**NOTE:** ArcGIS Pro is a Windows-based software and will NOT run on a Mac computer unless you have Parallels or Bootcamp installed. Contact Campus ITS in the Campus Store for more information.  

**NOTE:** Brock University has a site license for ArcGIS Pro. Therefore, you may download and install the software on any Windows machines for academic and research purposes. ArcGIS Pro can be found on any PC across campus. The Map, Data & GIS Library also has a special Alienware PC for use by the Brock community.  

Download the Excel file used in this tutorial. Niagara Sports Facilities acquired from [https://niagaraopendata.ca/dataset/niagara-sports-clubs-facilities](https://niagaraopendata.ca/dataset/niagara-sports-clubs-facilities). 

![image](https://user-images.githubusercontent.com/45638590/227005932-a60acb9f-3b34-4203-9088-5f012f652355.png)

OR...
The CSV is also available [here](NiagaraSportsFacilities.csv).  

----

## Geocoding with ArcGIS Pro

1. Run ArcGIS Pro on your Windows-based machine. Instructions for geocoding using ArcGIS Online follow the ArcGIS Pro tutorial.  
2. Sign in using your Brock credentials as per [this video](https://youtu.be/GqH4UHTUf2s) (NOTE: download instructions are also included in the video)
3. New Project > Map ![image](https://user-images.githubusercontent.com/45638590/227007092-cd43a99b-9b42-4152-a8ca-44f35939986f.png)  

4. Create a new project ("Geocoding Tutorial") and define the working directory (local storage is recommended).  
 ![image](https://user-images.githubusercontent.com/45638590/227007255-e290f578-fdfb-4353-a90b-6c9803f4e25b.png)  
 
5. Click OK. The software generates a new map project with a project folder and geodatabase.
6. By default there is a basemap projected to **WGS 1984 Web Mercator (auxillary sphere)**.
7. Click the **Map** tab at the top and click the **Add Data** button. ![image](https://user-images.githubusercontent.com/45638590/227008015-26c10409-bc60-42d9-ae8e-cdc336f8519f.png)  
8. Browse to the download directory holding the **NiagaraSportsFacilities.csv**. Select the file and click OK.
The table appears in the **Contents** pane under **Standalone Tables**:

   ![image](https://user-images.githubusercontent.com/45638590/227008580-a7c08919-b388-4492-9c60-3ec9ebc785f9.png)  

9. Right-click the table under **Standalone Tables** and click **Open**. Browse the attributes and notice the address fields. We will match the addresses in the table with the **Esri World Geocoder** to plot points on the map.
10. Close the table.
11. Right-click the table under **Standalone Tables** and click ![image](https://user-images.githubusercontent.com/45638590/227594718-e6fe8d94-7661-4e1f-ad61-d10eff85dc5b.png).  The **Geocode Table** wizard appears to the right of the map view. Navigate through the pages as follows.  
12. Page one outlines the steps involved. Click **Start** at the bottom of the page.  
13. **Step One**: from the **Input Locator** box, select **ArcGIS World Geocoding Service** ![image](https://user-images.githubusercontent.com/45638590/227595597-36186f55-7200-4d7c-881d-4f349f5f2063.png).  Click Next.

**NOTE: Geocoding consumes credits. Please contact maplib@brocku.ca before attempting to geocode a table with over 1000 records.**

14. **Step Two**: This page prompts you to identify how your data is structured. This particular table has the addresses stored in more than one field. Accept the default and click Next.  
15. In **Step Three**, the software attempts to match fields in the CSV with known fields in the address locator. Accept the defaults and click Next.  

   ![image](https://user-images.githubusercontent.com/45638590/227596541-53cc754f-600d-468c-893f-f85c14e88556.png)

16. For **Step Four**: **Output**, you can define where the resulting feature layer is created. Accept the defaults for now and click Next.  
17. For **Step Five**: Select Canada. This helps the software know the location more accurately. Click Next.    
18. For **Step Six**: Select the categories **Address** and **Postal** ![image](https://user-images.githubusercontent.com/45638590/227597232-6337b58a-fc04-4211-a982-95e1eaaf12eb.png).  Click Finish.  
19. From the summary page, notice the option at the top to calculate an estimate of how many credits will be consumed. Users at Brock University will have 300-500 credits by default. This activity will consume approximately **9 credits**.  
20. At the bottom of the page, click Run.  
21. When the process is finished, you will see a **Geocoding Completed** window. Here you will have the option to rematch any unmatched records. Click No.

   ![image](https://user-images.githubusercontent.com/45638590/227598587-38122e37-7632-4f78-96a7-a34d9aab67f6.png)  

The map now displays points representing sports facilities in the Niagara Region and you will see a new feature layer in the Contents pane on the left.  

   ![image](https://user-images.githubusercontent.com/45638590/227598970-e3f10177-21e4-44fe-ac40-f0077e1fc513.png)


## Geocoding with ArcGIS Online  

1. Go to [https://arcgis.com](https://arcgis.com) and sign in as per the instructions above. 

**NOTE: Geocoding in ArcGIS Online is limited to users with an organizational account.**

2. Click the **Map** option at the top of the screen. 

   ![image](https://user-images.githubusercontent.com/45638590/227601881-f0bf18bb-c6ee-4c59-b5d1-3c4d9dda8fe6.png)

This software as a service is constantly being updated. At the time of writing, the simplest way to plot points is to **Add layer from file**. Follow these steps:  

3. Click the little arrow beside the **Add** button ![image](https://user-images.githubusercontent.com/45638590/227602353-b3590aac-f145-4b7c-9c84-1ae88e13bb7a.png)  
4. Select the option to **Add Layer From File**.  
5. Click ![image](https://user-images.githubusercontent.com/45638590/227602648-f182d3b6-7677-4b8e-8045-881f9a8ba741.png)
6. Browse to your downloaded sports facilities table, select the csv and click Open. You will be taken through a series of prompts.
7. Select **Create a hosted feature layer and add it to the map.** Click Next.
8. This prompt allows you to identify the fields to include with the hosted feature layer. Accept the defaults and click Next. 
9. From the location settings, change the default selection to **Addresses or place names** ![image](https://user-images.githubusercontent.com/45638590/227603511-6799b99f-60cf-49ac-b77b-d2ba1436a683.png). 
10. Scroll down a bit and change the option for **Location Fields**. ![image](https://user-images.githubusercontent.com/45638590/227603839-ee48bcef-4e2a-4954-8814-20734007be2e.png). 
11. Scroll down to see how the software is matching the fields. You will need to select the field for Postal Code.
12. Scrolling down a little further will reveal approximately how many credits will be used to geocode the table.
 
   ![image](https://user-images.githubusercontent.com/45638590/227604218-ff42f5cd-6df7-41b3-9f8b-0b311919abf9.png)

13. Click Next. This page offers the option to change the layer name, storage location in ArcGIS Online and to add **Tags** (keywords) and a **Summary**.

   ![image](https://user-images.githubusercontent.com/45638590/227604646-efe7d799-0c48-4dd4-b25d-07455b5c0d99.png)

14. Click ![image](https://user-images.githubusercontent.com/45638590/227604709-afb779c6-512c-4829-927a-f0cc94ec3750.png). The results show the location of sports facilities across the Niagara Region.

   ![image](https://user-images.githubusercontent.com/45638590/227604891-4e6acf68-dd26-4a6f-9392-e7ae78bc7e72.png)



----

## Next Steps (Optional)
[Joining tabular data to geospatial data](https://brockdsl.github.io/ArcGIS_Joining_Data/)

----

**This tutorial is supported by the Brock University Research Lifecycle Department; Map, Data & GIS Library.  If you have any questions or concerns regarding this tutorial, don't hesitate to contact [maplib@brocku.ca](mailto:maplib@brocku.ca)**
