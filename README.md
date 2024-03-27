# Hankyung-Automation
Hankyung-article crawling and summarization, save, and upload automation projects.  
<br>

## Getting started
1. Obtain an API KEY from OPEN AI. Then, activate the Google Drive API in the Google Cloud console and download the ```credentials.json``` file. After that, place the json file in the same folder as the ```crawling.ipynb``` file.   
   - For more details, please refer to the link below.  
    https://developers.google.com/drive/api/quickstart/python?hl=ko

2. Create an .env file locally.
   - The .env file must contain ```OPENAI_API_KEY=...``` and ```FOLDER_ID=...```
   - <b><i>OPENAI_API_KEY</b></i> is the api key to use in openai
   - <b><i>FOLDER_ID</b></i> is the ID of the folder to use when uploading excel files to Google Drive.

3. Download the required libraries below.  
   (Or, uncomment the code starting with pip at the top of the crawling.ipynb file).

4. Run ```crawling.ipynb```.  
   If Google Drive malfunctions, test it in ```drive_test.ipynb```.  
  <br>

## Environments

### 1. Used
- Python (Jupyter Notebook)
- Selenium (Crawling)
- OpenAI  (Summarize with gpt-3.5-turbo API)
- GoogleDrive API v3 (Automate uploads)

### 2. Requirements
- python >= 3.10.7
- selenium >= 4.15.2
- webdriver-manager >= 4.0.1
- Google drive v3. API
    ```
    !pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib
    ```
- OpenAI API (openai >= 1.0.0)
  ```
  pip install openai
  ```
- openpyxl
  ```
  pip install openpyxl
  ```
- python-dotenv
  ```
  pip install python-dotenv
  ```


