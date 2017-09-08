<p align="center">
  <img src="https://github.com/StegSchreck/AngularCV/blob/master/src/assets/img/AngularCV.png" width="300px">
</p>

# AngularCV

This project serves the purpose of having a simple, self-hosted online-CV outside of LinkedIn, Xing, etc.

For a live demo, you can visit [cv.schreck.berlin](http://cv.schreck.berlin).


## Third party stuff 

It uses [AngularJS 4](https://angular.io/) and the [Material Design components for Angular](https://material.angular.io/).
Furthermore, the following third-party fonts are included:
* [Roboto](https://fonts.google.com/specimen/Roboto)
* [Roboto Slab](https://fonts.google.com/specimen/Roboto+Slab)
* [IcoMoon Free](https://icomoon.io/#preview-free)

The images in the `/src/assets/img/item-thumbnails` directory in this repository are property of their respective right owners and do not fall under the license of this repository. They're included for show-case purposes.

## Configuration

The CV items for the experience, education, projects and volunteering sections are configured in a JSON format in `/src/app/cv-item/cv-item.data.ts`.
Please notice the division of the education section, which is applied here. This enables you to re-arrange the the sections to your likings.

In the end, this is just an example of how it can be done. Feel free to take it as a template and adjust everything to your needs.

### Set your own data

Here is what you will have to change in order to adapt this project for yourself.

* `src/app/cv-item/cv-items.data.ts` contains all the configurable data for the page
  * You can use the current version as a template, but you will need to replace the data with your own
  * There are different use cases configured, so you can see different sets of data, which will be displayed differently in the rendered page
  * Some fields are required, for others there are checks in the frontend. Please try it yourself
* Replace `src/assets/img/avatar.jpg` with your profile picture (avatar)
* Replace `src/assets/img/cover.jpg` with an image for your overview page, imagine it as a kind of book cover
* Please delete all images in `src/assets/img/item-thumbnails` and add the ones you need (depending on what you configure in `src/app/cv-item/cv-items.data.ts`)
* Please delete all files in `src/assets/attachments` and add the ones you need (depending on what you configure in `src/app/cv-item/cv-items.data.ts`)
* Replace `src/favicon.ico`, it contains the icon your browser displays in the task bar

## AngularJS basics

See the [AngularJS basic guide](ANGULARJS.md) for the basics. For more information, visit the [AngularJS 4](https://angular.io/) website.

## Deployment to production

After you cloned/forked this project and adjusted it to your needs (and configuring with your data), you might want to deploy it in order to make it available to anyone.

See my [deployment guide](DEPLOYMENT.md) for a possible way how to achieve this with [Amazon Web Services (AWS)](https://aws.amazon.com/).
