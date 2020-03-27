# Instructions for the Pinterest Image Retrieval & Analysis Platform 
This web application uses a Pinterest API to retrieve data and images. It also provides functions to conduct some basic analysis of the images.

## Login Page
To get started you have to log in using your Pinterest email, username, and password. All of them have to be correct to pass the Pinterest authentication. If any of the credentials are incorrect, a notification will appear. Please retry and double check your user information on Pinterest if necessary.

## Search Page
### View and download user information
On the left of the screen, you will see all the information about your account. This is the data about your account that Pinterest stores on their server. If you press the “Download my Info” button, it will automatically return a .json file that contains all of the information shown on the left screen.
### Search Images
At the top of the page, you can input keywords into the query box and then click the “Search” button. As many as 150 of images will be retrieved; all the images will be displayed on the right part of the screen. 
### View Images Description
To see the description of the images, just hover over them with your cursor. The descriptions will be shown when you put your mouse on that specific image.
### View Images Metadata & Metadata Search
To see the larger version of the image, just click on the image thumbnail. The larger version of the image will pop up below the search bar. The following attributes of the image will be displayed:
-	Dominant Color 
-	Color Palette
-	Created Time
-	Grid Title
-	Is Promoted
-	Is Uploaded

There is more metadata associated with each pin. To search the specific metadata, just type in any letter in the search box under the “Pin Info” and it will show you any attributes that start with this letter. For example, if you want to see the board linked with this pin, just type in b and select “board”. **You have to press Enter to show the additional attributes.**
![](https://github.com/ReichYang/dil-pin/blob/master/search.png)


### Download Images to the Server
After you search for terms you can download the images to the server. This will enable you to conduct additional analyses on the images. Click the button called “Download Images to the Server,” and it will automatically move all the returned images to the platform server. The number of the pictures downloaded will show on the button after all the downloads have finished. **IMPORTANT: You must select "Download Images to Server" before you can conduct any analysis of them.**

### Redirect to the Image Analysis Page
After you have conducted one or more searches, click the “Go to the Analysis Page” button.

## Analysis Page
### Upload Google Vision Key (Under development)
We are currently working on tools that allow you to upload a Google Vision key so the web application can run more complex analyses on your images. At this point, the functionality may be limited or may return errors. To experiment, click the “Upload Key” button and select a google Vision API key ending with .json. Once you select the file to upload, the file name will appear below the button. **You have to press the “Submit” button so that the key file can be uploaded to the server.** The results of the upload, such as success or failure, will show after the page is refreshed.
### View Images in the Folder
You can view all the images downloaded from Pinterest. To do this, select the folder you want to peek in on the selection bar on the left of the screen, and then click “Peek in This Folder." All the images in this folder will be displayed at the bottom of the page, along with a tag indicating the number of the pictures in this folder.
### Download Images to Your Local PC
To download the images to your own PC, click on the button labeled “Download This Folder to Your Local PC.” A zip file containing all the images in your specified folder will be downloaded.
### Image Analysis
Our web application can show you some summary statistics about the images in a folder. To do so, simply click on the “Analyze This Folder” button, and the results will be shown on the right of the screen. Fifteen images in the selected folder will be analyzed. Make sure the folder is selected and its label turns blue. For now, the supported analysis includes:
-	Description Wordcloud
-	Domain Wordcloud
-	Board Wordcloud
-	Promoter Wordcloud
-	Date Graph
 
### Download Analysis Results
The analysis plots and their crude text data can be downloaded to your local PC as well. Click the "Download the Results" of the Analysis button and all the associated analysis files and plots will be zipped up and downloaded.
