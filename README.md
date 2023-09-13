# AWS-Lambda-Serverless

## Setting Docker Desktop in Mac

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

