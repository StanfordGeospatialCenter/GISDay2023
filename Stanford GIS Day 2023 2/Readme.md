### **Stanford GIS Day 2023**

Access link: <https://go.planet.com/gis-day-23>

### Setup

To follow each workshop, please sign into Colab at <https://colab.google/>. Follow steps for each workshop below.

For all workshops, you will need an API Key. To find your API Key:

1. Log in to your Planet account at <https://www.planet.com/explorer/>, and go to "My Account" by clicking on your initials on the top-right.
2. On the lefthand side of your account page, click on "My Settings"
3. Copy your API Key to use during each demo, this will authenticate your API calls by tying them to your account.

#### Workshop 1

1. Download the entire "Workshop 1" folder from NextCloud.
2. Upload "**lake-lagunita-large.geojson**" to your Google Drive.
3. Open Colab, go to File --> Upload Notebook, and upload "**REST_API_Intro.ipynb**". Open the notebook.
4. In Colab, run the following line to mount your drive:

```
from google.colab import drive
drive.mount('/content/drive')
```

5. On the lefthand side, click on the folder icon. Navigate through the folders to locate your "**lake-lagunita-large.geojson**" file ("content" -> "drive" -> "MyDrive" -> ?path to your file?)
6. Right-click the "**lake-lagunita-large.geojson.geojson**" file, select "Copy Path", and paste it into your notebook for the following line in the notebook:

```
geometry = parse_geojson("FILEPATH HERE")
```

#### Workshop 2

1. Download the entire "**Workshop 2**" folder from NextCloud.
2. Upload the entire "**Workshop 2**" folder to your Google Drive.
3. Open Colab, go to File --> Upload Notebook, and upload "**image_processing_with_python.ipynb**". Open the notebook.
4. Run the following line to mount your drive:

```
from google.colab import drive
drive.mount('/content/drive')
```

5. On the lefthand side, click on the folder icon. Navigate through the folders to locate your "**Workshop 2**" Folder ("content" -> "drive" -> "MyDrive" -> ?path to your folder?)
6. Right-click the "**Workshop 2**" folder, select "Copy Path", and paste it into your notebook for the following line:

```
data_dir = "PASTE PATH HERE"
```

7. Test imports and see if the `glob.glob` statements return filepaths for the geoms and data folders. You should be ready to follow along during Workshop 2!

#### Workshop 3

1. Download the entire "Workshop 3" folder from NextCloud.
2. Open Colab, go to File --> Upload Notebook, and upload "**planet_python_client_introduction.ipynb**". Open the notebook.

##### GEE Demo

We'll give a non-interactive demonstration of scripting in GEE with customized PlanetScope collections. If participants to not have a PlanetScope collection all steps can be repeated with Sentinel-2, a publicly available 10m resolution dataset. After the workshop feel free to repeat results by following these steps:

1. Sign up for Google Earth Engine.
2. Start a new script at <https://code.earthengine.google.com/>
3. From the "Workshop 3/GEE-sample-scripts" folder in NextCloud, download the following txt files: "**PlanetScope-shasta-GEE.txt**" and "**sentinel2-shasta-GEE.txt**"
4. Paste the contents of your selected txt file into the code editor.
   * If you've created a PlanetScope image collection, copy the contents of "PlanetScope-shasta-GEE.txt" into the editor. Import the collection and name the variable `ps_collection`
   * if you've not created a PlanetScope collection, try Sentinel-2's freely available data by pasting the contents of "sentinel2-shasta-GEE.txt" into the editor.
5. Remove the "//" comments for each section by highlighting a section and hitting "command + /". Uncomment and run sections to follow along.