# Changelog

# v0.52.0.0-220116
* `MODIFIED` Dose.Compare.cs refactor
* `MODIFIED` TheOptionObject.Finalize.cs refactor

# v0.51.0.0-220116
* `INFO` New version system
* `MODIFIED` Dose.Compare.cs refactor

# v0.28.22015.2329 (2022-01-15)
* `FIXED` Dose.cs had the old "Logging" configuration setting instead of "LogSetting"

# v0.28.22015.2319 (2022-01-15)
* `INFO` Code and comment cleanup/refactoring
* `FIXED` Still working on getting the new logging system to work correctly.

# v0.28.22015.2244 (2022-01-15)
* `INFO` Code and comment cleanup/refactoring
* `FIXED` Logs weren't being written because the username wasn't being passed.
* `REMOVED` InptAdmitDate project
* `REMOVED` NewDevelopment project

# v0.27.22011.1435 (2022-01-12)
* `INFO` Code and comment cleanup/refactoring
* `ADDED` Logfiles now have a development string at the end
* `ADDED` You can put a Xms pause between writing logfiles

# v0.26.22011.2136 (2022-01-11)
* `INFO` Code and comment cleanup/refactoring
* `ADDED` Logfiles are now written to the "Logs/<username>/logfile.mawslog"

# v0.26.22011.2039 (2022-01-11)
* `INFO` Code and comment cleanup
* `MODIFIED` RequestSyntaxEngine.RequestComponent.cs refactor
* `MODIFIED` RequestSyntaxEngine.TestFunctionality.cs refactor

# v0.26.22011.2012 (2022-01-11)
* `INFO` Code and comment cleanup
* `MODIFIED` MyAvatoolWebService.cs refactor

# v0.26.22011.1806 (2022-01-11)
* `INFO` Test build
* `ADDED` Dose.Compare only executes when the orderType is "Recurring"

# v0.25.22011.1722 (2022-01-11)
* `INFO` Test build
* `FIXED` Percentage logic was incorrect
* `FIXED` currentDose was sending an error when it should not have
* `MODIFIED` Modify error messages

# v0.25.22010.2222 (2022-01-10)
* `INFO` Test build
* `MODIFIED` Framework for missing dosage

# v0.25.22010.2207 (2022-01-10)
* `INFO` Test build
* `ADDED` Warning when a previous dose doesn't exist.
* `FIXED` Previous/current dose percentage logic was incorrect.

# v0.25.22010.2013 (2022-01-10)
* `INFO` Test build
* `MODIFIED` Reduced time between writing same-name log files from 500ms to 100ms
* `ADDED` 100ms pause between writing logfiles

# v0.25.22010.2008 (2022-01-10)
* `INFO` Test build
* `MODIFIED` Increased time between writing same-name log files from 100ms to 500ms

# v0.25.22010.2001 (2022-01-10)
* `INFO` Test build
* `MODIFIED` Added a "Process complete" log event

# v0.25.22010.1949 (2022-01-10)
* `INFO` Test build
* `MODIFIED` Changed logfile timestamp from "ffff" to "fffffff"

# v0.25.220110.1936 (2022-01-10)
* `INFO` Test build
* `MODIFIED` Removed "-{callerMemberName}" from logfile name

# v0.25.22010.1825 (2022-01-10)
* `INFO` Test build
* `MODIFIED` Added "-{callerLineNumber}" to logfile name
* `MODIFIED` Changed logfile timestamp from "fff" to "ffff"

# vv0.25.22010.1751 (2022-01-10)
* `INFO` Test build
* `MODIFIED` Logging changes (additional logging, modified syntax) for testing purposes.
* `MODIFIED` Updated AssemblyInfo files so all project versions match.
* `MODIFIED` Removed newline in warning message for dosing percentage

# v0.24.22007.1516 (2022-01-07)
* `INFO` Repository documentation updates

# v0.22.22005.1906 (2022-01-05)
* `INFO` Test build

# v0.21.22005.1914 (2022-01-05)
* `INFO` Test build

# v0.20.220103.HHMM (2022-01-03)

* `INFO` Repository documentation updates

# v0.20.220103.HHMM (2022-01-03)

* `INFO` Repository documentation updates

# 0.19.21312.1509 (2021-11-08)

* `MODIFIED` Utility.AppSettings.cs -> Utility.ExternalConfiguration.cs
* `MODIFIED` Config file is now sent as a filePath instead of a fileName, which will allow for more customization as to where the configuration file goes.

# v0.18.21307.1444 (2021-11-04)

* `INFO` Sourcecode comment updates

# v0.17.21306.1200 (2021-11-03)

* `INFO` Repository documentation updates

# v0.16.21207.1456 (2021-07-26)

* `INFO` Manual updates.

# v0.16.21200.2031 (2021-07-19)

* `INFO` Code and comment cleanup.

# v0.16.21200.1750 (2021-07-19)

* `INFO` Code and comment cleanup.
* `MODIFIED` **Dose:** The entire lastOrderScheduled text is parsed, instead of a specific line.
* `MODIFIED` **Dose:** Renamed lastOrderScheduled -> lastOrderSchedule
* `REMOVED` **NewDevelopment:** Settings.cs
* `REMOVED` **TheOptionObject:** Settings.cs
* `FIXED` **Utility:** The AppSettings class wasn't wrapped in a namespace.

# v0.15.21200.1703 (2021-07-19)

* `INFO` **Dose:** Dose.Compare.Percentage() works!

# v0.15.21200.1632 - 0.15.21200.1639 (2021-07-19)

* `INFO` Clean build for testing.

# v0.15.21200.1627 (2021-07-19)

* `INFO` Clean build for testing.
* `ADDED` **Dose:** formLoopCount and fieldLoopCount for debugging purposes.

# v0.15.21200.1537 (2021-07-19)

* `INFO` Clean build for testing.

# v0.15.21200.1526 (2021-07-19)

* `INFO` Clean build for testing.
* `FIXED` Putting the AssemblyVersion in the logfile contents was causing an issued. Roadmapped.

# v0.15.21200.1526 (2021-07-19)

* `INFO` Clean build for testing.

# v0.15.21200.1509 (2021-07-19)

* `INFO` Clean build for testing.
* `FIXED` *.settings* files were not renamed to *.conf* in the sourcecode. Duh.

# v0.15.21200.1455 (2021-07-19)

* `INFO` Clean build for testing.
* `ADDED` AppData/Configuration/
* `MODIFIED` **Utility:** WriteToFile() -> WriteTimestampedFile()

# v0.15.21200.1324 - v0.15.21200.1344 (2021-07-19)

* `INFO` A test for comment length (not project related)

# v0.15.21200.1316 (2021-07-19)

* `INFO` Code/comment cleanup
* `MODIFIED` Setting file extension is now *.conf*, since *.settings* was causing an issue with Visual Studio thinking it was a settings file.
* `ADDED` AppData/Configuration/

# v0.15.21196.1319 (2021-07-15)

* `INFO` Code/comment cleanup
* `ADDED` AppData/
* `ADDED` AppData/Logs/

# v0.15.21190.1333 (2021-07-09)

* `REMOVED` Logger project
* `REMOVED` Test project
* `REMOVED` MyAvatoolWebService.Settings.cs
* `MODIFIED` **Dose:** Percentages are now calculated as doubles.
* `MODIFIED` **Utility:** AppSettings.FromKeyValuePair() paramater changed to fileName, this way we can force the path to be either the production or staging folder.

# v0.15.21189.2018 (2021-07-08)

* `INFO` Clean build for testing.

# v0.15.21189.1853 (2021-07-08)

* `INFO` Clean build for testing.
* `ADDED` Basic Dose command functionality
* `MODIFIED` Renamed Dose.Verify.cs -> Dose.Compare.cs
* `ADDED` Settings for verifying dose information

# v0.15.21189.1822 (2021-07-08)

* `INFO` Initial v0.15 version.
* `INFO` Archived v0.14.

# v0.14.21189.1822 (2021-07-08)

* `INFO` Final v0.14

# v0.14.21189.1809 (2021-07-08)

* `INFO` Clean build for testing.

# v0.14.21189.1758 (2021-07-08)

* `INFO` Clean build for testing.

# v0.14.21189.1623 (2021-07-08)

* `INFO` Clean build for testing.

# v0.14.21189.1622 (2021-07-08)

* `INFO` Code/comment/documentation cleanup.
* `MODIFIED` **Utility:** AppSettings.FromKeyValuePair() now allows .settings files to have blank lines.
* `MODIFIED` **Utility:** LogEvent.WriteToFile() filename changed to make it easier to look at things in chronological order.

# v0.14.21189.1423 (2021-07-08)

* `INFO` Code/comment/documentation cleanup.
* `ADDED` **Utility:** Setting.cs
* `MODIFIED` **Utility:** Started migrating LogEvent code
* `MODIFIED` Logger.cs -> Utility.cs
* `REMOVED` **Dose:** Verify.Percentage_Testing.cs
* `REMOVED` **Dose:**Setting.cs (funcationality moved to Utility.AppSettings.cs)
* `REMOVED` **InptAdmtDate:** Compare.PreAdmitToAdmit_Testing.cs
* `REMOVED` **InptAdmtDate:** Setting.cs (funcationality moved to Utility.AppSettings.cs)

# v0.14.21188.1607 (2021-07-07)

* `WARN` This version doesn't work, I'm halfway through updating the logging functionality.
* `INFO` Code/comment/documentation cleanup.
* `ADDED` **Logger:** LogEvent.cs
* `ADDED` **Logger:** LogEvent.Timestamped()
* `REMOVED` **Logger:** Timestamped.cs, functionality moved to Logger.LogEvent.cs
* `MODIFIED` **Logger:** Started migrating LogEvent code
* `MODIFIED` Moved the stand-alone testing logic out of GetVersion(), and put it in it's own method. Now there is a single `//TestFunctionality()' line that is commented out by default, since it actually breaks MAWS in production.

# v0.14.21188.1355 (2021-07-07)

* `INFO` Initial v0.14 version.
* `INFO` Archived v0.13.
* `INFO` Archived v0.12.
* `INFO` Archived v0.11.
* `INFO` Archived v0.10.
* `INFO` Cleaned up dev/ archives.

# v0.13.21187.2038 (2021-07-06)

* `INFO` Clean build for testing.
* `MODIFIED` Removed custom lines in GetVersion().
* `MODIFIED` Fixed a few log comments.

# v0.12.21183.1411 (2021-07-02)

* `INFO` Final 0.12 version deployed to production for testing.
* `MODIFIED` Confirmed all projects are set to v0.12.21183.1411 

# v0.12.21183.0048 (2021-07-01)

* `INFO` Code/comment/documentation updates/cleanup
* `ADDED` Test case to the switch statement in RunScript()

## RequestSyntaxEngine

* `MODIFIED` Logging functionality brought up to other project levels
* `REMOVED` ParseRequest.cs

## NewDevelopment (previously TestFunctionality)

* `ADDED` Execute.cs
* `ADDED` Execute.Action()
* `ADDED` Settings.cs
* `ADDED` Settings.GetSettings()
* `REMOVED` Existing.cs
* `REMOVED` New.cs

# v0.12.21182.2257 (2021-07-01)

* `INFO` Code/comment/documentation updates/cleanup
* `ADDED` **Dose:** .licenseheader file
* `ADDED` **InptAdmitDate:** .licenseheader file
* `ADDED` **TestFunctionality:** .licenseheader file

# v0.12.21182.1839 (2021-07-01)

* `ADDED` **InptAdmitDate:** Compare.cs
* `ADDED` **InptAdmitDate:** Compare.PreAdmitToAdmit()
* `ADDED` **InptAdmitDate:** Execute.cs
* `ADDED` **InptAdmitDate:** Execute.Action()
* `ADDED` **InptAdmitDate:** Settings.cs
* `ADDED` **InptAdmitDate:** Settings.GetSettings()
* `ADDED` **Logger:** Logfiles now have the .mawslog extension
* `ADDED` **Dose:** Exectute.cs
* `ADDED` **Dose:** Exectute.Action()
* `ADDED` **Dose:** Settings.cs
* `ADDED` **Dose:** Settings.GetSettings()
* `ADDED` **Dose:** Verify.cs
* `ADDED` **Dose:** Verify.Percentage()
* `ADDED` **Dose:** Verify.Percentage_Testing()
* `REMOVED` Command project
* `REMOVED` MyAvatoolWebService.Dose.cs

# v0.12.21182.1554 (2021-07-01)

* `INFO` **Logger:** You can now specifiy what type of events are logged.
* `ADDED` **Logger:** Logger.LogEvent().
* `MODIFIED` **Logger:** Logging functionality for MyAvatoolWebService project.
* `MODIFIED` **Logger:** Log filenames and syntax.
* `ADDED` Dose project.
* `ADDED` InptAdmitDate project.

# v0.11.21181.1709 (2021-06-30)

* `INFO` Final v0.11 version deployed to production for testing
* `ADDED` New project: Command.csproj
* `ADDED` New project: TheOptionObject.csproj
* `ADDED` **Command:** InptAdmitDate.cs
* `ADDED` **Command:** InptAdmitDate.ExecuteAction()
* `ADDED` **Command:** InptAdmitDate.ComparePreAdmitToAdmit()
* `ADDED` **Command:** InptAdmitDate.ComparePreAdmitToAdmit_Testing()
* `ADDED` **Command:** TestFunctionality()
* `ADDED` **Command:** TestFunctionality.ForceInptAdmitDate()
* `ADDED` **Logger:** 10,000/sec to the filename.
* `ADDED` **Logger:** 10ms pause after writing a file.
* `ADDED` **Test:** Existing.cs
* `ADDED` **Test:** New.cs
* `ADDED` **TheOptionObject:** Finalize.cs
* `ADDED` **TheOptionObject:** Finalize.WhichComponents()
* `ADDED` **TheOptionObject:** Finalize.RequiredFields()
* `ADDED` **TheOptionObject:** Finalize.RecommendedFields()
* `ADDED` **TheOptionObject:** Finalize.NonRecommendedFields()
* `MODIFIED` **Logger:** Logger filename is more descriptive.
* `MODIFIED` Moved Test project to src/
* `REMOVED` **Logger:** *verboseLog* parameter. In roadmap.

# v0.11.21181.1407 (2021-06-30)

* `INFO` Code/comment/documentation updates/cleanup
* `MODIFIED` Moved Logger project to src/
* `FIXED` Project references.
* `ADDED` New project: Test.csproj
* `ADDED` *licenseheader* files
* `ADDED` **Logger:** *verboseLog* parameter
* `ADDED` **Test:** Existing.cs
* `ADDED` **Test:** Existing.Force()
* `REMOVED` Testing.cs

# v0.11.21181.1305 (2021-06-30)

* `INFO` Code/comment/documentation updates/cleanup
* `MODIFIED` **Logger:** Timestamped.WriteToFile(): *logMessage* is now an optional parameter, and defaults to "No log message defined".
* `MODIFIED` **Logger:** Minor changes to log output text.
* `MODIFIED` **Logger:** Renamed the "Caller" parameters to be more descriptive.

# v0.11.21179.1755 (2021-06-28)

* `INFO` Groundwork for framework update
* `MODIFIED` Lots of logging updates
* `ADDED` New project: Dose.csproj
* `ADDED` New project: Logger.csproj
* `ADDED` New project: InptAdmitDate.csproj
* `ADDED` New project: RequestSyntaxEngine.csproj
* `ADDED` **Logger:** Timestamped.cs
* `ADDED` **Logger:** Timestamped.Maintenance()
* `ADDED` **Logger:** Timestamped.WriteToFile()
* `ADDED` **RequestSyntaxEngine:** ParseRequest.cs
* `ADDED` **RequestSyntaxEngine:** ParseRequest.ExecuteCommand()
* `ADDED` **RequestSyntaxEngine:** RequestComponent.cs
* `ADDED` **RequestSyntaxEngine:** RequestComponent.GetCommand()
* `ADDED` **RequestSyntaxEngine:** RequestComponent.GetAction()
* `ADDED` **RequestSyntaxEngine:** RequestComponent.GetOption()
* `ADDED` **RequestSyntaxEngine:** TestFunctionality.cs
* `ADDED` **RequestSyntaxEngine:** TestFunctionality.Force()
* `REMOVED` Maintenance.cs
* `REMOVED` Logger.cs

# v0.10.21176.1652 (2021-06-25)

* `INFO` Code/comment/documentation updates/cleanup
* `FIXED` A completed OptionObject wasn't being passed back to Avatar.

# v0.10.21176.1518 (2021-06-25)

* `INFO` Code/comment/documentation updates/cleanup
* `ADDED` Settings.cs
* `ADDED` Settings.GetSettings()
* `ADDED` Settings are now loaded from an external file
* `ADDED` "TestFunctionality" setting
* `MODIFIED` \MAWS\Log -> \MAWS\Logs
* `MODIFIED` Testing.Force() -> Testing.Functionality()

# v0.9.21179.1515 (2021-06-28)

* `FIXED` Fixed returning the OptionObject.

# v0.9.21179.1312 (2021-06-28)

* `ADDED` Added Dose in switch statement, for testing Dose functionlity.

# v0.9.21176.0200 (2021-06-25)

* `INFO` Final v0.9 release. Fixed a few things that impacted deployment.

# v0.9.21172.1617 (2021-06-21)

* `INFO` Final v0.9 release (not the case, see above)

# v0.9.21172.1316 (2021-06-21)

* `INFO` Code/comment/documentation updates/cleanup
* `REMOVED` MyAvatoolWebService.ForceTest()
* `ADDED` Testing.cs
* `ADDED` Testing.Force()
* `MODIFIED` MAWS Request commands/actions/options are now converted to lowercase prior to being returned by RequestSyntaxEngine.cs
* `MODIFIED` Maintenance.ConfirmLogDirectory() -> Maintenance.ConfirmLogDirectory()

# v0.9.21172.1210 (2021-06-21)

* `INFO` Code/comment/documentation updates/cleanup

# v0.9.21171.1735 (2021-06-20)

* `MODIFIED` Added [DEBUG] prefix to log files
* `MODIFIED` Added [SYSTEM] prefix to log files

# v0.9.21171.1731 (2021-06-20)

* `ADDED` Error logging for invalid commands
* `ADDED` Error logging for invalid InptAdmitDate.cs actions
* `ADDED` Error logging for invalid Dose.cs actions

# v0.9.21171.1719 (2021-06-20)

* `INFO` Code/comment cleanup (lots of undocumented changes to *InpatientAdmissionDate* to bring it in-line with the new framwork)
* `MODIFIED` Renamed *InpatientAdmissionDate* -> *InptAdmitDate*
* `MODIFIED` Removed *GetRequestAction()* and *GetRequestOption()* from *MyAvatoolWebService.asmx.cs* so the scope is tightened up a bit.
* `ADDED` /Resources/Log/
* `ADDED` Maintenance.cs
* `ADDED` Maintenance.CreateLogDirectory()
* `ADDED` Logger.cs
* `ADDED` Logger.WriteToTimestampedFile()
* `ADDED` Dose.cs
* `ADDED` Dose.ForceTest()
* `ADDED` Dose.VerifyPercentage()
* `ADDED` Dose.VerifyPercentage_Testing()
* `MODIFIED` Convert actions/options to lowercase

# v0.9.21170.2311 (2021-06-19)

* `INFO` Re-implemented the *InpatientAdmissionDate* command
* `ADDED` InpatientAdmissionDate.cs
* `ADDED` RequestSyntaxEngine.ForceTest()

# v0.9.21170.2044 (2021-06-19)

* `INFO` Built-in (simplistic!) testing works.
* `ADDED` MyAvatoolWebService.ForceTest()
* `ADDED` RequestSyntaxEngine.ForceTest()

# v0.9.21170.1739 (2021-06-19)

* `INFO` Documentation updates

# v0.9.21170.1726 (2021-06-19)

* `INFO` Documentation updates
* `MODIFIED` Started the change to the MAWS Request Syntax Engine

# v0.9.21170.1628 (2021-06-19)

* `INFO` Code/comment/documentation changes

# v0.9.21161.1940 (2021-06-10)

* `ADDED` OptionObjectMaintenance.cs
* `ADDED` OptionObjectMaintenance.FinalizeObject()
* `ADDED` OptionObjectMaintenance.FinalizeRequiredFields()
* `ADDED` OptionObjectMaintenance.FinalizeNonRequiredFields()

# v0.9.21161.1854 (2021-06-10)

* `INFO` Code and comment cleanup

# v0.9.21161.1834 (2021-06-10)

* `INFO` Version refresh

# v0.9.21161.1831 (2021-06-10)

* `ADDED` MyAvatoolWebService.GetVersion()
* `ADDED` MyAvatoolWebService.RunScript()
* `ADDED` MyAvatoolWebService.MethodName()

# v0.9.21161.1816 (2021-06-10)

* `INFO` Added the NTST.ScriptLinkService.Objects project to the solution
* `MODIFIED` MAWS Manual updates

# v0.9.21161.1749 (2021-06-10)

* `INFO` Framework commit

# v0.8.21111.1535 (2021-04-21)

* `ADDED` /Resources/Dev/sourcecode-information.md
* `RENAME` /Resources/Dev/current-versions.md -> /Resources/Dev/developent-information.md

# v0.8.21111.1434 (2021-04-21)

* `ADDED` /Resources/Dev/current-versions.md

# v0.7

* `INFO` Update documentation/comments.

># v0.6

* `INFO` Update documentation/comments.

# v0.5

* `INFO` Update documentation/comments.

# v0.4

* `INFO` Update documentation/comments.

# v0.3

* `INFO` Update documentation/comments.

# v0.2.21014.1544 (2021-01-14)

* `ADDED` OptionObjectMaintenance.cs
* `ADDED` OptionObjectMaintenance.Complete()
* `ADDED` OptionObjectMaintenance.CompleteRequired()
* `ADDED` OptionObjectMaintenance.CompleteRecommended()
* `ADDED` OptionObjectMaintenance.CompleteNotRecommended()
* `ADDED` Functionality to InptAdminDate.VerifyPreAdmitDate() so once the "typeOfAdmissionField" and "preAdmitToAdmissionDateField" fields are found, MAWS stops looking through the sentOptionObject2. This should speed things up in some cases.
* `MODIFIED` Refactored detailed error messages in InptAdminDate.VerifyPreAdmitDate() with string interpolation.

# v0.2.21014.1544 (2021-01-14)

* `ADDED` InptAdminDate.Parser() method
* `ADDED` InptAdminDate.VerifyPreAdmitDate() method
* `MODIFIED` Requests in the RunScript() method now uses "workingOptionObject2" instead of "completedOptionObject2" because I want to make sure it's very clear as to what MAWS is sent ("sentOptionObject2"), what it works with ("workingOptionObject2"), and what it returns to myAvatar ("completedOptionObject2").
* `RENAMED` "InptAdminDate.cs" to "InptAdmitDate.cs" because this request will do things with the inpatient *admission* date, and the "Admin" abbreviation indicates *administration*.
* `RENAMED` "action" to "mawsRequest" because going forward ScriptLink events will be passing a "request-action" (e.g., "InptAdmitDate-VerifyPreAdmitDate")
* `UPDATED` Documentation

# v0.2.21014.1425 (2021-01-14)

* `REMOVED` Local methods to pre-process an action (i.e., "MyAvatoolWebService.asmx.cs.InptAdminDate"). The pre-processing is now going to be done in the action class, in a method named "Parser()" (e.g., "InptAdminDate.Parser()").
* `UPDATED` Documentation

# v0.2.21013.1802 (2021-01-13)

* `ADDED` InptAdminDate.cs class.
* `MODIFIED` Renamed "MyAvatoolWebService.asmx.cs.MethodName()" to "MyAvatoolWebService.asmx.cs.InptAdminDate()".
* `MODIFIED` Added "InptAdminDate" case to the switch statement in RunScript().
* `MODIFIED` Added "SubPolicyNumber" case to the switch statement in RunScript().

# v0.1.21013.1420 - 0.1.21013.1712 (2021-01-13)

* `ADDED` MAWS.licenseheader file for use with the [License Header Manager](https://marketplace.visualstudio.com/items?itemName=StefanWenig.LicenseHeaderManager) extension.
* `MODIFIED` AssemblyInfo.cs with...uh...assembly information.
* `MODIFIED` Renamed *sentOptionObject* to *sentOptionObject2* so it's more inline with Netsmart's (wierd) naming conventions.
* `ADDED` MAWS.licenseheader file for use with the [License Header Manager](https://marketplace.visualstudio.com/items?itemName=StefanWenig.LicenseHeaderManager) extension.
* `MODIFIED` AssemblyInfo.cs with...uh...assembly information.
* `MODIFIED` Renamed *sentOptionObject* to *sentOptionObject2* so it's more inline with Netsmart's (wierd) naming conventions.

# v0.0.0.0 (2021-01-12)

* `INFO` This is a blank MAWS template (built following the steps in the MAWS [manual](doc/man/manual-custom-myavatar-web-services.))

<br>

## [Back to MAWS documentation](../doc/)&nbsp;&nbsp;|&nbsp;&nbsp;[Back to MAWS repository](https://github.com/spectrum-health-systems/MyAvatoolWebService)