---
title: "Activate Katalon Studio Enterprise"
sidebar: katalon_studio_docs_sidebar
permalink: katalon-studio/docs/activate-KSE.html
redirect_from:
    - "/katalon-studio/docs/katalon-studio-activation-since-70.html#activating-katalon-studio-enterprise"
    - "/katalon-studio/docs/katalon-studio-activation-since-70.html#other-options"
    - "/katalon-studio/docs/katalon-studio-activation-since-70.html#activating-katalon-studio-enterprise-trial-license"
description:
---
You need a license to activate Katalon Studio Enterprise (KSE) that can work with or without an Internet connection.

> Having activation problems? [Click here.](https://docs.katalon.com/katalon-studio/docs/troubleshoot-activation-problems.html)

## Online Activation

You can activate KSE in an online environment with the [trial KSE license](/katalon-studio/docs/license.html), or an online license that grants permission to the registered users.

* Trial License: When you first download Katalon Studio version 7.0.0 and log in to your Katalon account, the trial license associated with your account is automatically activated. Each trial KSE license is tied to each Katalon account.
* Online License: Only the registered users who are added to the **Register Users** list can use online licenses.

In the **Katalon Studio Activation** window:

1. Enter the email and password registered for your Katalon account then click **Activate**.
2. You are navigated to your organization, or you can select one of the organizations you belong to in the drop-down list, click **OK**.
3. You are recommended to install the plugins for a better experience with Katalon Studio.
4. Open an existing project or create a new one in Katalon Studio.
5. In Katalon TestOps Integration pop-up window:

* Select a team in the configured organization that you have permission to access.
* Select a project under that team you’d like to work on or create one if you have permission.

### Configuring proxy for online activation

If you are behind a Proxy Server, you need to configure the Authentication proxy settings before activating KSE. Click **Configure Authentication Proxy** at the bottom of the Activation dialog box.

<img src="https://github.com/katalon-studio/docs-images/raw/master/katalon-studio/docs/proxy-preferences/config-proxy-activation.png" width="">

In the Proxy Settings dialog box, you can select one of three options below.

* **Use system proxy configuration**: Katalon Studio tries to guess which proxy server your system is behind and sync with these settings.
* **No proxy**: there's no proxy.
* **Manual proxy configuration**: you can manually set up your proxy.

## Offline Activation

A machine ID is required for generating an offline license. In the Katalon Studio Activation window, click **Offline Activation**:

1. **Generate an offline license**: Log into [Katalon Admin](https://admin.katalon.com/) > go to your organization > **License** > **Katalon Studio Enterprise** > **Create Offline License** > insert a **Machine ID** > click **Create**.

    > Notes:
    >
    >* Machine ID is granted for each computer installing Katalon Studio. In the Katalon Studio Activation window, click **Offline Activation**, you can view and copy your machine ID.
    >* Only organizational owners or admins can access **License** in an organization. Learn more about [Roles and Permission](https://docs.katalon.com/katalon-analytics/docs/user-management.html#roles-and-default-permissions).

2. **Locate the generated license**: To use a license, click the **Download** button, the license will be downloaded as a `KSE_<machine_ID>.lic` file. Then click **Browse** in **Katalon Studio Enterprise Activation** to locate the downloaded license file.

3. Click **Activate**.

### Other options

After activating KSE, there will be a window requiring you to log into your Katalon account for connecting to [Katalon TestOps](https://docs.katalon.com/katalon-studio/docs/katalon-analytics-beta-integration.html) and [Store](https://docs.katalon.com/katalon-store/docs/overview.html).

KSE users can use plugins both from Store and [offline](https://docs.katalon.com/katalon-studio/docs/offline-plugin.html).
