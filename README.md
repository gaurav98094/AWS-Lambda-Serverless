# AWS-Lambda-Serverless

## Project Architecture

<img src="images/project.jpeg">


### Setting Docker Desktop in 
<hr>

To install Docker on a Mac, you can use Docker Desktop, which provides a user-friendly interface and makes it easy to run and manage Docker containers on macOS. Here's how you can install Docker on your Mac:

1. **Check System Requirements**:

   Before you begin, make sure your Mac meets the following requirements:

   - macOS must be running macOS Yosemite 10.10.3 or later.
   - Your Mac must have a 64-bit Intel CPU (Apple Silicon is not officially supported as of my last knowledge update in September 2021).
   - Virtualization must be enabled in your BIOS/UEFI settings if it's not already enabled.

2. **Download Docker Desktop**:

   Visit the Docker Desktop for Mac download page: [Docker Desktop for Mac](https://www.docker.com/products/docker-desktop) and click on the "Download for Mac" button. You may need to create or sign in to your Docker Hub account to access the download.

3. **Install Docker Desktop**:

   Once the Docker Desktop .dmg file is downloaded, open it by double-clicking. Drag the Docker icon into your Applications folder. This will install Docker Desktop on your Mac.

4. **Run Docker Desktop**:

   After installation, open Docker Desktop from your Applications folder. It will prompt you for your system password to complete the installation process.

5. **Enable Docker**:

   Docker Desktop will start running, and you'll see the Docker icon in your Mac's menu bar. Click on it, and you can access Docker settings and status.

6. **Test Docker Installation**:

   Open a terminal window and run the following command to check if Docker is installed and running properly:

   ```bash
   docker --version
   ```

   You should see the Docker version information if it's installed correctly.

7. **Run a Test Container**:

   To test Docker further, you can run a simple container:

   ```bash
   docker run hello-world
   ```

   This command will download a small Docker image and run a container from it. If everything is set up correctly, you should see a message confirming that your installation appears to be working correctly.

That's it! You've successfully installed Docker on your Mac using Docker Desktop. You can now start creating and managing containers on your macOS system.

<hr>

### Create IAM User


1. **Sign In to AWS Console**:

   Log in to your AWS Management Console using an account with administrative privileges.

2. **Open IAM Dashboard**:

   Once you're logged in, navigate to the IAM (Identity and Access Management) service by searching for "IAM" in the AWS Management Console search bar or by selecting it from the "Security, Identity, & Compliance" section.

    <img src="images/iam1.png">

3. **Create a New IAM User**:

   In the IAM dashboard, select "Users" from the left-hand navigation pane and then click the "Add user" button.

4. **Configure User Details**:

   - Enter the username for the new IAM user.
   - Choose the type of access. For this example, select "Programmatic access" (to allow the user to interact with AWS via APIs) and "AWS Management Console access" (to allow access to the AWS Management Console).
   - Optionally, you can set a custom password or let AWS auto-generate one.
   - You can require the user to reset their password on their first login for security reasons, or you can choose not to enforce a password change.
   
   <img src="images/iam2.png">
   

5. **Permissions**:

   In the "Set permissions" step:
   
   - Select "Add user to group" and choose an existing group with administrator access policies (e.g., the built-in "Administrators" group). This is the fastest way to give the user administrator access.
   - Alternatively, you can attach policies directly to the user by selecting "Attach existing policies directly." In this case, search for and attach the "AdministratorAccess" policy, which provides full administrative access.

   <img src="images/iam3.png">

6. **Tags (Optional)**:

   You can add tags to the user if needed. Tags are key-value pairs that help you categorize and manage users.

7. **Review**:

   Review the user details, permissions, and settings to ensure they are correct. If everything looks good, click the "Create user" button.

8. **Success**:

   You will see a confirmation page with the user's access keys (if programmatic access was enabled). Make sure to save these credentials securely because you won't be able to see the secret key again.

9. **Send Welcome Email** (Optional):

   If you provided an email address during user creation, you can send a welcome email with login details to the user. This step is optional.

That's it! You've successfully created an IAM user with administrator access in AWS. This user will have full access to AWS services and resources, so be sure to manage their credentials securely.
