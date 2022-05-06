<!-- 220328.094653 -->

<h1 align="center">

  <img src="../../resource/image/logo/MAWS-logo-512x350.png" alt="MyAvatool Web Service logo" width="256">
  <br>
  Manual
  <br>

</h1>

<h6 align="center">
  Last updated: March 28, 2022
</h6>

***

<h3 align="center">

  [Home](manual.md)&nbsp;&bull;&nbsp;[Getting started](manual-getting-started.md)&nbsp;&bull;&nbsp;[Hosting](manual-hosting-maws.md)&nbsp;&bull;&nbsp;Importing&nbsp;&bull;&nbsp;[Using](manual-using-maws.md)&nbsp;&bull;&nbsp;[ScriptLink](manual-scriptlink-events.md)&nbsp;&bull;&nbsp;[Additional information](manual-additional-information.md)

</h3>

***

#### CONTENTS
[Overview](#overview)<br>
[Importing MAWS into your environment](#importing-maws-into-your-environment)<br>

# Overview
In order for myAvatar™ to use MAWS, you'll need to import MAWS into your myAvatar™ environments.

## Before you begin
To continue with this documentations, you will need to know the location of MAWS in your environment.

# Importing MAWS into your environment
Importing MAWS into your myAvatar™ environments is pretty simple. Here is how you do it.

## Confirming the MAWS WSDL
Before attempting to import MAWS into myAvatar™, you should make sure that you have a valid **W**eb **S**ervice **D**escription **L**anguage (**WSDL**) URL. To do this, paste the URL of the MAWS WSDL in a web browser and attempt to access the URL.

For example, pointing a browser to `https://your-organization.com/MyAvatoolWebService.asmx?WSDL` should display XML that looks something like this:

<h6 align="center">

  <img src="img/wsdl-xml-example-799x393.png" width="600">
  <br>
  An example of a WSDL file
  <br>

</h6>

If the WSDL file *is diplayed* in the browser, that URL is what you are going to need going forward.

If the WSDL file *is not displayed*, you'll need to get a valid WSDL location before continuing.

## Importing the MAWS WSDL
Any form can be used to import a web service, and once a web service has been imported it can be used by any form that allows ScriptLink events.

We will use the *Admissions* form to import the MAWS WSDL:
1. Open the **Form Designer** form
2. Choose the "Admissions" form from the **Forms** dropdown
3. Choose the XXX tab from the **Tabs** dropdown
4. Click the **Show Tab** button
5. You will now see the form tab in designer mode. In the upper left of myAvatar™ you will see a **Settings** button:

<h6 align="center">

  <img src="img/scriptlink-form-designer-settings-button-364x335.png" width="300">
  <br>
  The "Settings" button.
  <br>
</h6>

6. Clicking the **Settings** button will bring you to the ScriptLink options page. Right now we are interested in the **Import WSDL for ScriptLink** section:

<h6 align="center">

  <img src="img/scriptlink-options-import-wsdl-847x375.png" width="747">
  <br>
  The ScriptLink options page.
  <br>
</h6>
<br>

7. Copy/paste the MAWS WSDL URL into the **Import WSDL for ScriptLink** field in myAvatar™
2. Click the **Import** button.

You should get a popup letting you know the WSDL was imported successfully.

# Next step: How to use MAWS
Before you write ScriptLink events, you'll want to know [how MAWS works](manual-using-maws.md).