## Part 0 - Starting the Server & Registering a Manifest

This section contains a couple of very basic files which will become the basis of our extensions. There is a simple HTML page which includes jquery and some other libraries, a javascript file where we will write our code, and an empty css file. At the end of the section, we'll be able to see our extension show up in Tableau, and load this basic html page inside a dashboard.

#### Starting the Server

Extensions are simply web pages, so the first thing we'll need to do is make sure we have a web server up and running to serve our content. To do that, navigate to the root of the extensions repository in a command prompt, and run `npm start`. This command will start a simple http server listening on port 8765 and just serving up the contents of this repository over http.

#### Registering the Manifest

The very first thing you need to do is to provide an extension, or manifest file (`.trex`). If you cloned or downloaded the `.zip` file for the repository, you can find the manifests for the tutorial inside the Manifests folder. The `.trex` file contains basic information like the name of the extensions (as it will appear in Tableau) and the url where the extension is hosted. To have the extension show up in Tableau, you must copy the `.trex` file into your `My Tableau Repository (Beta)/Extensions` fodler and restart Tableau. When Tableau start up again, you should see the extensions listed when authoring a dashboard.

#### Testing It Out

After starting the server, copying the manifest file over, and restarting Tableau, you should now see your extension in the dashboard authoring pane on the left side of Tableau. Drag out the extension onto a dashboard, and you should see "Hello Extensions" on your dashboard.

![Part 0 Screenshot](../assets/Part_0.png)

[Next Section (Part 1 - Initialization)](../Part_1/readme.md)