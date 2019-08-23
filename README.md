## Setup

### Sign-in to Required Accounts

1. Sign into GitHub: <a href="https://github.com/login" target="_blank">Github</a>
2. Sign into Codenvy: <a href="https://codenvy.io/site/login" target="_blank">Codenvy</a>

### Creating a New GitHub Repo For Your Site

GitHub will host a website for each user and organization for free.  The feature is called <a href="https://pages.github.com/" target="_blank">GitHub Pages</a>.

The first thing we need to do is create a new repository on GitHub and name it using the following naming pattern:

    yourusername.github.io
    
<a href="https://github.com/new" target="_blank">Click here to open a new browser tab and create create a new GitHub repository</a>.

NOTE: If you're not signed-in to GitHub, you might see a web page that says 404 (This is not the web page you are looking for).  Just sign-in to GitHub on this page and you will be forward to the _create new repository_ page.

Follow these steps and see the screenshot below to create a new repository.

1. On the Create New Repository page, in the box for **Repository name**, name the repository like:

    `your-github-username.github.io`
    
    replacing `your-github-username` with you actual GitHub username.  MAKE SURE your username is spelled correctly, otherwise you'll have problems **(See A)**.
    

2. Enter a description for your repository in the **Description** box, like `My own awesome website!' **(See B)**.

3. Select the **Public** radio button to allow anyone to see this repository **(See C)**.

4. Check the **Initialize this repository with a README** box **(See D)**.

5. Click the **Add .gitignore** button, and Search for "Node". Click on "Node" from the dropdown. **(See E)**.
    
6. Double check that you have followed these instructions properly. Then click **Create Repository** **(See F)**.

**Click to enlarge image**
<img src="https://raw.githubusercontent.com/magdalenemc/first-website/edit1/img/create-repo.png">

Awesome, you created your repository!

### Creating a Codenvy Workspace for our Website Project

GitHub is where we store and version our code. Codenvy is where we edit our code.  COdenvy is web-based set of tools for creating software.  By working in the cloud, our projects workspace is independent from any one computer. 

Follow these steps and see the screenshot below to create a new workspace.

1. Sign into Codenvy.io
2. On the left sidebar, go to "Workspaces"
3. Click on "Add Workspace"
    A) Name: "operation-spark"
    B) Team: "personal"
    C) Select Stack: All
    D) Scroll down until you find "Ubuntu"
    
Once you have followed these steps you can create your workspace

<img src="img/codenvy-create-workspace-part-1.png">

### Cloning repository from Github to Codenvy Workspace

1.  Next step, we need to _clone_ our repository into our Cloud9 workspace, where we will do our work.  After creating the repository on GitHub, you'll be brought to the repository's default view.  In the top right corner of the screen, you will want to:
    
    A) Click Clone or download (See A). Make sure that "Clone with HTTPS" appears in the top right corner of the dropdown box. PLEASE NOTE: THIS STEP IS IMPORTANT! Make sure Clone with HTTPS is selected! IF it is not, an option to select it should appear in the top right corner of the dropdown box.
    
    B) Click the "Copy URL to clipboard" button (See B).
    
    <img src="https://raw.githubusercontent.com/magdalenemc/first-website/edit1/img/copy-repo-url.png"> 


2. On the left sidebar, go to "Workspaces". Click on "Add Workspace"

    A) Name: "operation-spark"
    
    B) Team: "personal"
    
    C) Select Stack: All
    
    D) Scroll down until you find "Ubuntu"
      
    Once you have followed these steps you can create your workspace
    
3. Clone your Github repository into your Codenvy workspace by copy/pasting this command into the terminal at the bottom of your workspace (replace `"my-github-url.github.io"` with your own github url that you copied from step 1):

`git clone "my-github-url.github.io`

## Install `opspark` tool

1. Enter this command:

`curl https://raw.githubusercontent.com/creationix/nvm/v0.25.0/install.sh | bash`

2. Close your terminal. Select **Run** from the top Menu. Click on **Terminal**

3. Back in your terminal, enter these commands:

```
nvm install 8
nvm alias default 8
npm install -g opspark
os login
```

4. When prompted, enter your Github username and password.

## Lesson Steps

### TODO 1 : Create index.html

Right-click in the file system and select `New File`

<img src="https://raw.githubusercontent.com/OperationSpark/first-website/master/img/create-new-file.png">

Name the file, `index.html`, (press return after naming it to save the new name) like so:

<img src="https://raw.githubusercontent.com/OperationSpark/first-website/master/img/name-it-index.png">

Next, double click the `index.html` file to open it so we can begin editing the file, like so:

<img src="https://raw.githubusercontent.com/OperationSpark/first-website/master/img/open-index-html.png">

Ok great!  We've created our `index.html` file and opened it in the text editor to start developing our website!
