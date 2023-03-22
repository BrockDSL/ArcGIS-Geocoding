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
6. By default there is a basemap projected to **WGS 1984 Web Mercator (auxillary sphere)**
7. Click the Map tab at the top and click the Add Data button ![image](https://user-images.githubusercontent.com/45638590/227008015-26c10409-bc60-42d9-ae8e-cdc336f8519f.png)  
8. Browse to the download directory holding the NiagaraSportsFacilities.csv Select the file and click OK.
The table appears in the Contents pane under Stand Alone Tables:

![image](https://user-images.githubusercontent.com/45638590/227008580-a7c08919-b388-4492-9c60-3ec9ebc785f9.png)










----

## Next Steps (Optional)
This is where you can add any additional resources, follow up tutorial, or workshop reccomendations that users might use to continue learning about the tool described in the tutorial.  The more the better!

----

**End notes**
This is where you mention the DSL, MDGL, or Research Lifecycle department and put in contact information.  An example of what this might look like is:

**This tutorial is supported by the Brock University Research Lifecycle Department.  If you have any questions or concerns regarding this tutorial, don't hesitate to contact [DSL@Brocku.ca](mailto:DSL@Brocku.ca)**
