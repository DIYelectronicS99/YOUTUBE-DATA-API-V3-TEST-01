# YOUTUBE-DATA-API-V3-TEST-01
uploads a local video to youtube using python script
setup:
Set up command line by:

$ cd youtube-upload-master
$ sudo python setup.py install

---

1. Python installed and environment variables set correctly.
2. Enabling youtube data api in google console with a google account and activating oauth client for getting client secret json and id
3. Use this JSON as your credentials file: --client-secrets=CLIENT_SECRETS.json file
4. sample command to upload a video :

  youtube-upload --title="your tite" " --description="description" --category="Music" --tags="sdaufhsfh" --client-secret="my_client_secret.json"  /*(DO NOT USE CLIENT SECRET'S'.JSON !!! USE THE JSON INFO , AMKE A FILE CALLED client_secret.json   AND USE THAT WITH THE FOLLOWING SYNTAX )*/ --playlist="NAME OF PLAYLIST YOU WANT TO ADD TO/EXISTING PLAYLIST"  localfilepathofvideo/videofilename.mp4/mkv/flv/any video format
  
  5. Add the following inside youtube-upload-master\youtube_upload\main.py :
    from oauth2client import file
  6. Save the file and run the commans previously stated.
  
This will get your said video uploaded to your channel. While running the code for the first time, a link pops up in the command window, click that and it shows a verification code. Once done, you're free to upload videos.


---

Notes:

    1.Main logic of the upload: main.py (function upload_video).
    1.Check the Youtube Data API.
    3.Some Youtube API examples provided by Google.
