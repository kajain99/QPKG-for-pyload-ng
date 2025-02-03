# What It Is

This is a QPKG package designed to simplify the installation of **pyLoad-ng** on QNAP NAS devices. It leverages **QNAP's Container Station** and the official **linuxserver/pyload-ng** Docker image to provide a seamless experience for managing and automating downloads. This QPKG ensures compatibility with QNAP systems while utilizing Docker for easy deployment and maintenance.

# What It Needs

To use this QPKG, you will need:

* A **QNAP NAS** with **Container Station** installed and configured.
* **App Store configured to allow unsigned applications.** Since this QPKG is unsigned, you need to allow installation from unverified sources. This is safe as long as you download the QPKG from a **trusted source** like this GitHub repository.
* **Internet access** to download the necessary Docker images.

# How to Install

## Step 1: Enable Unsigned Package Installation
Since this QPKG is unsigned, you need to allow the installation of unsigned applications:

1. Open your **QNAP App Center**.
2. Navigate to **Settings > General**.
3. Check the option **Allow installation of applications without valid signatures**.

## Step 2: Install the QPKG

1. Download the **pyLoad-ng QPKG** from the [Releases](https://github.com/YOUR_REPOSITORY/releases) section.
2. In the **QNAP App Center**, click **Install Manually**.
3. Select the downloaded **QPKG file** and follow the on-screen instructions.

## Step 3: Initial Run

1. Once installed, start the **pyLoad-ng** application from the QNAP App Center.
2. Open a web browser and go to:
   ```
   http://<your-qnap-ip>:8181
   ```
   *(Replace `<your-qnap-ip>` with your QNAP’s IP address, e.g., `192.168.1.100`.)*

## First-time login credentials and changing password 

Login with the default username and password:

**Username:** `pyload`

**Password:** `pyload`

Change your password by going to settings>user>change password 

## Step 4: Configure Download Paths

By default, **all QNAP shares are mounted under `/mnt`** inside the container. To configure your download directories:

1. Go to **pyLoad Web UI**.
2. Navigate to **Settings > General > Download Folder**.
3. Set it to a preferred location, e.g., `/mnt/my_dir`.

# Credits

- **Built with QNAP's QDK Kit**.
- **Powered by the official linuxserver/pyload-ng Docker image**: [linuxserver/pyload-ng](https://hub.docker.com/r/linuxserver/pyload-ng).

Enjoy **pyLoad-ng** on your QNAP NAS!

