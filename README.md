# GitHub Hosted Site Template

A template repo for sites created using Typerefinery app and hosted on GitHub pages site.

You can use this template to create a new GitHub reop that will contain your site content. This template contains the necessary configuration to get you started quickly.

You can use CMS in the Typerefinery app to create and edit content for your site. When you are ready, you can publish and deploy your site to GitHub pages. You can use CMS to edit and publish your changes when you need to update site content. The Typerefinery app will push your changes to GitHub, and GitHub Actions pipeline will deploy these to GitHub pages.

Having CMS running on your local PC will ensure that you have all the control and tools needed to create whatever you desire.

Typerefinery CMS uses the latest Bootstrap to give you a great starting point for your site. You can use the built-in Bootstrap components to create your site. You can also use the built-in Bootstrap components to create your own components and extend the CMS functionality.

***
NOTE: TypeRefinery is in early development and is not yet ready for production use. Currently, it's only installable on Windows. 

Mac and Linux support is coming soon, please leave a comment on [Mac](https://github.com/typerefinery-ai/typerefinery/issues/501) and [Linux](https://github.com/typerefinery-ai/typerefinery/issues/502) tickets to hurry us along.
***
## Usage

Follow this guide to create a new GitHub page site from this template. Install and configure Typerefinery application to use it's built-in CMS to create and deploy your site to GitHub pages.

### Create a new repository from this template

1. Click the `Use this template` button on the github page.
2. Set the repository name and description.
3. Click the `Create repository from template` button.
4. Click the `Code` button and copy the HTTPS repository Url and save it.

### Update the repository settings

1. Click the `Settings` button.
2. Click the `Pages` tab.
3. Select `Deploy from a branch` branch in `Source` dropdown.
4. Select `main` branch in `Branch` dropdown and press `Save` button.

### Update the repository details

1. Click the `Gears` button in the About section.
2. Tick the `Use your GitHub Pages website` checkbox and click `Save changes` button. Link to your new site will appear in the About section.

### Create a personal access token

1. Go to the [New personal access token (classic)](https://github.com/settings/tokens/new) page.
2. Set the token `Note`.
2. Select `No expiration` in `Expiration` field.
3. In `Select scopes` tick `public_repo` in the `repo` section.
5. Click the `Generate token` button.
6. Copy the generated token and save it.

### Download and install Typerefinery

1. Go to the [Typerefinery Latest Release](https://github.com/typerefinery-ai/typerefinery/releases/latest) page.
In the Assets section, download the installer for your platform.
3. Install the app.
4. Run the app.
5. Wait for the app to finish setting up your services.
6. When you see Ready in the app, open a web browser and open CMS Homepage on [http://localhost:8113].

### Create new Site

1. In a web browser, open CMS Homepage on [http://localhost:8113](http://localhost:8113).
2. Login with the default credentials: `admin` and `admin`.
3. Click the `Create space` button and choose `Pages`.
4. Set the space `Title`, lowercase `Name`, and select `Typerefinery pages` in `Template`.
5. Click on the newly created space.

### Create new Space Config

1. Click `Create page` button.
2. On `Template selection` choose `Space Config` template.
3. On `Page properties` on `General` tab:
    * set the page `Title` to `Space Config`, and 
    * set `Name` to lowercase `_admin`.
4. On `Page properties` on `Deploy` tab:
    * select `Github` in `Deploy Target`, and
    * in `Additional Paths to Publish` add a new Path entry with `/apps/typerefinery/clientlibs`.
5. On `Page properties` on `Github` tab:
    * paste your repository Url into `Repository URL` field in format `https://github.com/user/repo.git`.
    * paste your personal access token into `Personal Access Token` field.
    * set the `Branch` field to `main`.
    * set User and Email field to your desired user and email identifiers that will be used to push content to this repo.

### Create home page

1. Click `Create page` button.
2. On `Template selection` choose `Page` template.
3. On `Page properties` on `General` tab:
    * set field `Title` to `Home`, and
    * set field `Name` to lowercase `index`.
4. Click `Create` button.

### Publish space

1. In a web browser, open CMS Homepage on [http://localhost:8113](http://localhost:8113).
2. On your new space click on the `...` button and select `Publish space`.
3. On `Publish space` dialog select `All` in `Publish Options`, click on `Deploy after Publish` toggle, and click `Publish` button.
4. Wait for the space to be published and deployed.
5. Check GitHub repository `main` branch for the new files.

## FAQ

### My site is not deploying

If you get errors publishing your site, please check the following before seeking support.

### Problems Publishing

* You did not create `_admin` page in the root of your space.
* You did not provide all the config values on GitHub tab in page properties of `_admin` page.
* You don't have an account on Github
* You didn't do the email verification to complete your account on Github
* Your username does not have push rights to that repository (e.g. your username is not listed as a contributor)
* You used the wrong username by accident (substituting with one that does not have push rights on that repository)
* You entered the password wrong
* You pushed using the wrong protocol (e.g. you used SSH or HTTPS, when only the other protocol was acceptable)
* You provided the correct authentication but the email address you sent with it did not match what the server was expecting

### Can't see all content or styles

* You did not publish the space after creating the content.
* You did not deploy the space after publishing the content.
* You did not provide all the config values on GitHub tab in page properties of `_admin` page.
* You did not add `/apps/typerefinery/clientlibs` in `Additional Paths to Publish` in page properties of `_admin` page on the Deploy tab.

### I don't see the "Use this template" button on the GitHub page. What should I do?

Ensure that you are logged in to your GitHub account. If you still don't see the button, make sure you have the necessary permissions to create repositories from templates.

### I encountered an error while creating the repository from the template. What could be the problem?

Double-check your internet connection and try again. If the error persists, ensure that you have not reached any limits on your GitHub account, such as repository creation limits.

### After setting up the repository, I can't find the "Settings" button. Where is it located?

The "Settings" button is usually located at the top-right section of your repository page, near the "Code" button. If you don't see it, ensure that you have sufficient permissions to access repository settings.

### I selected the "Deploy from a branch" option, but I don't see the desired branch in the "Branch" dropdown. What should I do?

Ensure that you have pushed the desired branch to your repository. If the branch is missing, try refreshing the page or check if you have permission to access that specific branch.

### I updated the repository details, but I don't see the link to my new site in the About section. What could be wrong?

Double-check that you correctly enabled the "Use your GitHub Pages website" checkbox in the repository settings. If it still doesn't appear, make sure you saved the changes properly and refresh the page.

### I'm unable to generate a personal access token. What could be causing this issue?

Check your GitHub account settings to ensure that you have the necessary permissions to generate personal access tokens. If the problem persists, contact GitHub support for further assistance.

### Typerefinery installation failed. What should I do?

For now, Typerefinery only supports Windows. Please leave a comment on [Mac](https://github.com/typerefinery-ai/typerefinery/issues/501) and [Linux](https://github.com/typerefinery-ai/typerefinery/issues/502) tickets to hurry us along. Double-check that you downloaded the correct installer for your platform. 

### The CMS Homepage on http://localhost:8113 is not accessible. How can I resolve this?

Verify that the Typerefinery app is running and fully set up and that all services in the app are running. Ensure that you entered the correct URL in your browser.

### I can't log in to the CMS Homepage with the default credentials. What should I do?

Double-check that you are using the correct username and password. 

### I encountered errors while publishing and deploying the space. How can I troubleshoot this issue?

Check your internet connection stability. Ensure that you provided the correct repository URL and personal access token in the Space Config settings. Verify that your GitHub account has the necessary permissions for repository deployment. Review any error messages received during the publishing and deployment process.

### Still stuck?

If you are still stuck, make a video of what you are trying to do, get a zip of your logs, and leave them in a comment on [Bugs installing the app](https://github.com/typerefinery-ai/typerefinery/issues/503) issue.