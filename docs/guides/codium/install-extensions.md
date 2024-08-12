---
title: "How to Manually Install Codium Extensions: A Step-by-Step Guide"
subtitle: "Easily Install VSIX Files in Visual Studio Code (Codium) Without the Marketplace"
description: "Learn how to manually install Visual Studio Code (Codium) extensions with this comprehensive guide. Whether you're working offline, testing pre-release versions, or simply need an alternative to the marketplace, this step-by-step tutorial will walk you through downloading and installing VSIX files for a seamless coding experience."
icon: simple/vscodium
status: new
---

# How to Manually Install Codium Extensions

Visual Studio Code (Codium) is a powerful and popular code editor that supports a vast range of extensions. While the easiest way to install extensions is through the built-in marketplace, there may be times when you need to manually install an extension. This guide will walk you through the steps to manually install Codium extensions.

## Prerequisites

Before you begin, ensure you have the following:

- **Codium** installed on your system.
- **Internet access** to download the extension files.
- **Basic knowledge** of navigating your operating system’s file structure.

## Step 1: Download the Extension File

1. Visit the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/vscode) in your web browser.
2. Search for the extension you want to install.
3. Click on the extension to open its detail page.
4. Scroll down to the "Resources" section and click on the “Download Extension” link.
5. The extension will be downloaded as a `.vsix` file, which is the format for Codium extensions.

<figure markdown>
  ![Image title](https://shardbyte.com/assets/images/guides/codium/codium-gif-001.gif){ width="800" }
  <figcaption>Download the Extension</figcaption>
</figure>

!!! note
    If the "Download Extension" link is not available, you can append `?preview=true` to the URL of the extension's detail page and press Enter. This often reveals the download link.

## Step 2: Install the Extension in Codium

Once you have the `.vsix` file, follow these steps to install it:

1. Open **Codium**.
2. Click on the **Extensions** view icon on the Sidebar (or press `++Ctrl+Shift+X++` on your keyboard).
3. In the Extensions view, click the three-dot menu at the top-right corner.
4. Select **Install from VSIX...** from the dropdown menu.
5. Navigate to the folder where you downloaded the `.vsix` file, select it, and click **Open**.

<figure markdown>
  ![Image title](https://shardbyte.com/assets/images/guides/codium/codium-gif-002.gif){ width="800" }
  <figcaption>Install the Extension</figcaption>
</figure>

Your extension will now be installed and ready to use.

## Step 3: Verify the Installation

After installing the extension, it’s important to verify that it was installed correctly:

1. In the Extensions view (`++Ctrl+Shift+X++`), type the name of the installed extension in the search bar.
2. If the extension appears in the list with an "**Uninstall**" or "**Disable**" button, it has been successfully installed.
3. You can now begin using the extension features as described in its documentation.

<figure markdown>
  ![Image title](https://shardbyte.com/assets/images/guides/codium/codium-gif-003.gif){ width="800" }
  <figcaption>Confirm the Extension</figcaption>
</figure>

## Additional Tips

- **Offline Installation:** If you're working in an offline environment, you can transfer the `.vsix` file to the offline machine and follow the installation steps.
- **Updates:** Manually installed extensions won’t receive automatic updates. To update, you’ll need to download and install the newer version manually.

## Conclusion

Manually installing Codium extensions is a straightforward process that gives you greater control over your development environment. Whether you're installing an extension on an offline machine or trying out a pre-release version, these steps will help you get up and running quickly.
