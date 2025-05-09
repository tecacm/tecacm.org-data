![TecACM Banner](./images/tecACM_banner.png?raw=true)

## TecACM.org Data 
This repository holds the data which our chapter's website uses to load such as images or files we might update frequently like our events list, this with the purpose of not having to update the site as often and instead just editing a couple of json files.


### Important Files:
##### Make sure these are syntactically valid json files before pushing any changes, otherwise you *will break* the site until they're fixed

- chapter_members.json is self explanatory, it contains the relevant information about the current team leading the chapter. 
- groups.json contains information about groups that we as a team administrate, such as the competitive programming club or our hackathon HackMTY, including links to our Linktr.ees
- events.json contains a list of events that we are organizing at the moment. 
- The images directory contains the images we may not want to upload to our page such as events because they might be temporary. However as to not strain github (and for loading time concerns), we use jsdelivr to load images instead.


### How to upload an image:
To use an image from here on the site you could use the raw file directly from github, but we reccomend you instead use jsdelivr. You can use this https://www.jsdelivr.com/github after uploading the image to the repository and pushing it to the remote. However that would involve two commits, one for uploading the image, and another one for updating events for example. But as you will soon notice the path pretty much stays the same always, https://cdn.jsdelivr.net/gh/tecacm/tecacm.org-data@main/images/events/image_here.webp so you can just replace `image__here.webp` with your file's name and extension but that will pretty much always work (assuming your image is under images/events, if it's not you should change that too). 