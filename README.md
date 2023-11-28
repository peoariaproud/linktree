# Peoria Proud Link Tree
This repository holds all the code necessary to deploy a statically generated, linktree-style website.

## Configuring the Link Tree
All site configuration is done in the `hugo.toml` configuration file. Updating any information in here (and updating any other file) will cause the site to automatically rebuilt and re-deployed.

## Adding/Updating Buttons
To add a new button to the site:
1. Open the `hugo.toml` file at the root of the project
1. Look under links section that starts with `links = [`
    * Each link looks something like this: `{ facebook = "https://www.facebook.com/peoriaproud" }`
    * the first part `facebook`, determines which icon to show on the button
    * the second part `"https://www.facebook.com/peoriaproud"` determines where the button links to.
    * the third part is optional, but you can add custom button text by copying what is done on the website button and changing it: `{ web = {href = "https://peoriaproud.org", text = "Website"}}`
1. The links show on the website in the order they appear in this list, insert your link wherever you want it to show up in the list.

## Static Site Advantages
Statically generated websites offer several notable benefits. First, they boast enhanced performance and speed since the pages are pre-rendered and served directly to the user, reducing server processing time and load. Second, they offer improved security due to the absence of a database or dynamic software on the server, making them less vulnerable to common web attacks. Third, they are easier to scale because static files can be distributed across multiple servers or through a Content Delivery Network (CDN) with ease. Fourth, they often result in lower hosting costs since they require less server resources and computing power. Finally, they provide a more reliable and consistent user experience, as the pre-rendered content ensures that all users receive the same content regardless of server load or dynamic elements.
