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

  [Home](manual.md)&nbsp;&bull;&nbsp;[Getting started](manual-getting-started.md)&nbsp;&bull;&nbsp;[Hosting](manual-hosting-maws.md)&nbsp;&bull;&nbsp;[Importing](manual-importing-maws.md)&nbsp;&bull;&nbsp;[Using](manual-using-maws.md)&nbsp;&bull;&nbsp;ScriptLink&nbsp;&bull;&nbsp;[Additional information](manual-additional-information.md)

</h3>

***

# ABOUT SCRIPTLINK
When working with custom web services and myAvatar™, it's inevitable that you will hear about ScriptLink. And depending on who/what is describing what ScriptLink is/does, you are going to get different answers.

Netsmart tends to use "ScriptLink" as another way to say "custom web services", but that's not really the case. I mean, a "custom web service" is a web service. It's in the name. ScriptLink *isn't* a web service.

As far as I can tell, ScriptLink is simply a link to a script. Or, more specifically, a link to a custom web service. Or, *even more specifically*, something that calls a method in a custom web service when something is done with/on a form in myAvatar™.

To summarize, ScriptLink is essentially a line of code in the form designer that kicks off the magical stuff you've written in a custom web service.

# CREATING SCRIPTLINK EVENTS
Before you can use MAWS (or any custom web service) with myAvatar™, make sure you've [imported](manual-importing-maws.md) it.

To use the MAWS with myAvatar™, you will need to add a ScriptLink event to a form event. When that event takes place, myAvatar™ will pass information to MAWS (and potentiall recieve something back).

You can add a ScriptLink event to the following form events:
* when the form loads ("Form Load")
* after the submit button is clicked, but prior to filing the form ("Pre-File")
* after the submit button is clicked and the form has been filed ("Post-File")

#### What about other form events?
You can also use custom web services with fields and controls, but that is beyond the scope of this documentation.

#### Forms that can't use ScriptLink events
A list will go here.

## ADDING A SCRIPTLINK EVENT TO A FORM
Let's say you wanted to have MAWS do something when you hit the **Submit** button on form. To do that you would:
1. Open the **Form Designer** form
2. Choose the myAvatar™ form you want to use from the **Forms** dropdown
3. Choose the form tab from the **Tabs** dropdown
4. Click the **Show Tab** button
5. You will now see the form tab in designer mode. In the upper left of myAvatar™ you will see a **Settings** button:

<h6 align="center">

  <img src="img/scriptlink-form-designer-settings-button-364x335.png" width="300">
  <br>
  The "Settings" button (again)
  <br>

</h6>

6. Clicking the **Settings** button will bring you to the ScriptLink options page:

<h6 align="center">

  <img src="img/scriptlink-event-example-839x369.png" width="739">
  <br>
  The ScriptLink options page (again, but this time for something different)
  <br>

</h6>
<br>

Next we will need to choose an event that will call the Avatool Web Service, and determine the action that will take place. For this example, we will call the *VerifyInpatientAdmissionDate* action on the form's *Pre-File* event:

7. Click the dropdown in the **Pre-File** row under the **Available Scripts** column
8. Choose **AvatoolWebService** (the *red* box)
9. Type "VerifyInpatientAdmissionDate" in the **Pre-File** row under the **Script Parameter** column (the *purple* box)
10. Uncheck the **Disable All Scripts For Form** and **Disable All Scripts on Error** boxes  (the *green* box)
11. Click **Return to Designer** (the *yellow* box), and the ScriptLink options page will close, and you will be back on the **Tab Designer** page
12. Click the **Save** button, and you bw returned to the **Form Designer** page
13. Click **Submit**

Now, when the Admission form is submitted, myAvatar™ will ask MAWS to VerifyInpatientAdmissionDate for a specific client.

## DISABLING SCRIPTLINK EVENTS
Disabling the functionality of a custom web service is simple and quick, and you can choose to disable individual ScriptLink events, or all ScriptLink events on a form.

In addition, enabling/disabling ScriptLink events does not require any downtime for your environments. The change is made when you hit **Submit**.

To do either of those, you would:
1. Open the **Form Designer** form
2. Choose the myAvatar™ form you want to use from the **Forms** dropdown
3. Choose the form tab from the **Tabs** dropdown
4. Click the **Show Tab** button
5. You will now see the form tab in designer mode. In the upper left of myAvatar™ you will see a **Settings** button:

<h6 align="center">

  <img src="img/scriptlink-form-designer-settings-button-364x335.png" width="300">
  <br>
  The "Settings" button.
  <br>

</h6>

6. Clicking the **Settings** button will bring you to the ScriptLink options page:

<h6 align="center">

  <img src="img/scriptlink-event-example-839x369.png" width="739">
  <br>
  The ScriptLink options page.
  <br>

</h6>
<br>

### Disabling specific ScriptLink events
If you want to disable a specific ScriptLink event:
1. Check the **Disable** boxes  (the *green* box) next to the **Form Load**, **Pre-File** and/or **Post-File** events
2. Click **Return to Designer** (the *yellow* box), and the ScriptLink options page will close, and you will be back on the **Tab Designer** page
3. Click the **Save** button, and you bw returned to the **Form Designer** page
4. Click **Submit**

Now, when the form is submitted, myAvatar™ *will not* process ScriptLink events for the events you have disabled.

### Disabling all ScriptLink events on a form
If you want to disable all ScriptLink events on a form:
1. Check the **Disable All Scripts For Form** and **Disable All Scripts on Error** boxes  (the *green* box)
2. Click **Return to Designer** (the *yellow* box), and the ScriptLink options page will close, and you will be back on the **Tab Designer** page
3. Click the **Save** button, and you bw returned to the **Form Designer** page
4. Click **Submit**

Now, when the Admission form is submitted, myAvatar™ *will not* process *any* scriptlink event on the form.

## SCRIPTLINK TESTING SUGGESTIONS
It is strongly recommended that you thouroughly test any custom web service functionality in your environments, and that includes MAWS.

Since it's easy to enable/disable ScriptLink events, my suggestions when testing functionality is to:
* Enable functionlity after the business day has started
* Disable functionality prior to the business day ending
* Test during business hours for a week

Using the above suggestions, you will be able to disable functionlity quickly if there are any issues.

# THAT'S IT!
You've hosted MAWS, imported it into myAvatar™, and added ScriptLinks to forms.

If you are still curious about MAWS, check out the [additional information](manual-additional-information.md) document.