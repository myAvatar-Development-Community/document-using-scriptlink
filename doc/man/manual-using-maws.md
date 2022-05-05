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

  [Home](manual.md)&nbsp;&bull;&nbsp;[Getting started](manual-getting-started.md)&nbsp;&bull;&nbsp;[Hosting](manual-hosting-maws.md)&nbsp;&bull;&nbsp;[Importing](manual-importing-maws.md)&nbsp;&bull;&nbsp;Using&nbsp;&bull;&nbsp;[ScriptLink](manual-scriptlink-events.md)&nbsp;&bull;&nbsp;[Additional information](manual-additional-information.md)

</h3>

***

#### CONTENTS
[Overview](#overview)<br>
[About MAWS requests](#about-maws-requests)<br>
[Actions and Commands](#actions-and-commands)<br>
[How to make a MAWS request](#how-to-make-a-maws-request)<br>
[MAWS request results](#maws-request-results)<br>
[Valid MAWS requests](#valid-maws-requests)<br>

# OVERVIEW
Once you have [hosted](manual-hosting-maws.md) MAWS and [imported](manual-importing-maws.md) it into your myAvatar™ environment, it's ready to use by making a `mawsRequest`.

# ABOUT MAWS REQUESTS
A `mawsRequest` consists of an `action` and a `command` for MAWS to perform against data received from myAvatar via an *OptionObject2*.

Each `mawsRequest` is formatted like so: `%action%-%command%`

## EXAMPLES

* The `InptAdmitDate-VerifyPreAdmitDate` request verifies that a clients pre-admission date is the same as the system date. The request **action** is `InptAdmitDate`, and the request **command** is `VerifyPreAdmitDate`. 

* The `SubPolicyNumber-TrimWhitespace` removes leading/trailing whitespace from a subscriber policy number. The request **action** is `SubPolicyNumber`, and the request **command** is `TrimWhitespace`. 

# ACTIONS AND COMMANDS
## ACTIONS ARE CLASSES
Each `mawsRequest` action has a corresponding sourcecode class with the same name.

For example, any `InptAdmitDate` actions will be handled by the *InptAdmitDate.cs* class.

## COMMANDS ARE METHODS
Each `mawsRequest` command has a corresponding method with the same name. This method can be found in the action's class sourcecode. 

For example, the `VerifyPreAdmitDate` **command** of the `InptAdmitDate` **action** would be processed by the *VerifyPreAdmitDate()* method in the *InptAdmitDate.cs* class.

# HOW TO MAKE A MAWS REQUEST
To perform an `mawsRequest`, you'll need to create a ScriptLink event in myAvatar that passes the request and an *OptionObject2* to MAWS. For more information about creating ScriptLink events, please see the MAWS [manual](manual-scriptlink-events).

# MAWS REQUEST RESULTS
A `mawsRequest` will result in one of the following:

1. Prompt the user to make a change within myAvatar
2. Warn the user about something
3. Optionally return modified data to myAvatar

# VALID MAWS REQUESTS

## INPATIENT ADMISSION DATE

#### `InptAdmitDate-VerifyPreAdmitDate`

**What it does**<br>
Verifies that the Inpatient Admission Date is the same as the system current date.

**How it works**<br>
* When a completed Admission form is submitted, we check to if the "Admission Type" is "Pre-Admission"
* If the "Admission Type" is set to  "Pre-Admission" and the "Pre-Admission Date" is not the same as the system date, a pop-up will notify the user that they need to modify the Pre-Admission Date field  to equal the system time, and the user will be returned to the form to modify the Pre-Admission Date
* If the "Admission Type" is not set to "Pre-Admission", or if it is and the Pre-Admission Date is the same as the system date, the form is submitted normally

## SUBSCRIBER POLICY NUMBER

#### `SubPolicyNumber-TrimWhitespace`

**What it does**<br>
TBD.

**How it works**<br>
* TBD
* TBD
* TBD

# NEXT: CREATING SCRIPTLINK EVENTS
Now that you know how MAWS *works*, you can start adding [ScriptLink events](manual-scriptlink-events.md) to your myAvatar™ forms.