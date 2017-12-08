# Zuck.js with Hasura Data API

This is a static webpage implemented with Hasura as backend for the volume. This webpage uses [zuck.js](https://github.com/ramon82/zuck.js/) to provide the "status","story" functionality to the webpage.

This quickstart repo comes with the following things:
* A sample "stories" database consisting of sample details needed for the story
* A static webpage making use of Hasura Data API (jQuery) to fetch details from the stories table.

![Preview]
(https://raw.githubusercontent.com/anirudhmurali/zuckjs-stories/master/stories.png)

Your app will be running at https://www.cluster-name.hasura-app.io

## To edit the content of the stories:

1. Open Hasura API Console with ```hasura api-console```
2. Go to the Data section
3. Select ```stories``` > Insert Row
4. You'll see the below table layout:

![Preview]
(https://raw.githubusercontent.com/anirudhmurali/zuckjs-stories/master/stories2.png)

5. Provide the URL of the image in the ```photo``` field.
6. The ```items``` field takes the following JSON:

```[{"length":3,"seen":false,"time":"12-10-03","linkText":false,"link":"","src":"https://pbs.twimg.com/profile_images/899612476274114561/79RSAFw7.jpg","preview":"https://pbs.twimg.com/profile_images/899612476274114561/79RSAFw7_400x400.jpg","id":"Hasura","type":"photo"}]```

Edit the ```length``` entry to change the duration of the story
Edit the first image source to change the story content
Edit the second image source to change the preview of the story

7. Click 'Save' to insert the row, refresh your webpage to see the new story.
8. Edit ```zuck.js``` and refer the [official library documentation](https://github.com/ramon82/zuck.js/) for more implementation with this library.
9. Have fun!
