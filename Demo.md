<a name="title" />
# WAAD Authentication #

---
<a name="Overview" />
## Overview ##

1. File / New / Configure WAAD in a new project.
1. Showcase the GeekQuiz solution with WAAD Authentication
1. Deploy or show portal configuration in an already deployed site

<a id="goals" />
### Goals ###
In this demo, you will see how to:

1. (TODO: Insert goal 1 here)
1. (TODO: Insert goal 2 here)
1. (TODO: Insert goal 3 here)

<a name="technologies" />
### Key Technologies ###

- {TODO: Include technology name here} [here][1]
- {TODO: Include technology name here}
- [{TODO: Include technology name here}][2]

[1]: http://insert_link_to_technology_1_here/
[2]: http://insert_link_to_technology_2_here/

<a name="Setup" />
### Setup and Configuration ###
Follow these steps to setup your environment for the demo.

1. Follow the steps detailed in [this link](http://docs.nuget.org/docs/creating-packages/hosting-your-own-nuget-feeds) to setup local sources for the following directories:

	* **C:\Program Files (x86)\Microsoft Web Tools\Packages**
	* **C:\Program Files (x86)\Microsoft ASP.NET\ASP.NET Web Stack 5\Packages**

	![NuGet Sources](Images/nuget-sources.png?raw=true)

1. Open Visual Studio 2013.
1. Open the **GeekQuiz.sln** solution located under **source\begin**.
1. If you don't have one, create a user account for the application. To do that, press **F5**, click **Register** and provide the information required. After that, close the browser window.

	> **Note:** Remember the information you provided as you will be using it during the demo.

1. In Visual Studio, close all open files.

<a name="Demo" />
## Demo ##
This demo is composed of the following segments:

1. [Creating a new organization web site](#segment1).
1. [Running the organization's GeekQuiz](#segment2).

<a name="segment1" />
### Creating a new organization web site ###

1. Open the **File / New Project** dialog and show the options in the **Visual C# / Web** section.

1. Name the application _GeekQuiz_ and click **OK**.

	![Creating a new project](images/creating-a-new-project.png?raw=true "Creating a new project")

	_Creating a new project_

1. Select new **MVC** project and check the **Web API** option.

1. Click **Change Authentication** button.

	![Updating the authentication method](images/updating-the-authentication-method.png?raw=true "Updating the authentication method")

	_Updating the authentication method_

	> **Speaking Point:** VS tooling allows you to enable WAAD authentication easily. All you need is to provide your tenant domain name and administrator credentials, the two-way trust between your WAAD tenant and your web application is automatically configured

1. On **Change Authentication** dialog, select **Organizational Accounts** option.

	![Selecting the Organizational Accounts option](images/selecting-organizational-accounts.png?raw=true "Selecting the Organizational Accounts option")

	_Selecting the Organizational Accounts option_

1. 	Expand the first combo box in order to showcase the different posibilities.
	
	![Showing the organization account types](images/showing-the-organization-types.png?raw=true "Showing the organization account types")

	_Showing the organization account types_

1. 	Expand the **Access Level** combo box in order to showcase the different posibilities.

	![Showing the access level posibilities](images/showing-the-access-level-options.png?raw=true "Showing the access level posibilities")

	_Showing the access level posibilities_

1. Enter your domain (ex. "mydomainname.onmicrosoft.com") as **Domain**.

	![TODO](images/updating-the-domain.png?raw=true "TODO")

	_TODO_

1. Expand the **More Options** dialog by clicking the button at the end of the dialog.

	![Showing more options](images/showing-more-options.png?raw=true "Showing more options")

	_Showing more options_

1. Click **OK** to continue.

	![Completing the authentication update](images/completing-the-authentication-update.png?raw=true "Completing the authentication update")

	_Completing the authentication update_

1. Sing in using an admin account for your organization (ex. "admin@mydomainname.onmicrosoft.com")

	![Signing in with an organization admin account](images/signing-in-with-an-organization-admin-account.png?raw=true "Signing in with an organization admin account")

	_Signing in with an organization admin account_

1. Back in **New ASP.Net Project** dialog, click **Create Project** button.

	![Completing the project creation](images/creating-the-project.png?raw=true "Completing the project creation")

	_Completing the project creation_

	> **Speaking Point:** VS tooling configures two-way trust relationship between your app and your WAAD tenant. Your app is registered as a Relying Party of the tenant; and the tenant is configured as an Identity Provider of the app.

1. **CTRL+F5** to run the web site.

1.	Sign in using a user account for your organization (ex. "user@mydomainname.onmicrosoft.com").

	![Signing in using one of the organization's user account](images/logging-in-with-an-organization-user.png?raw=true "Signing in using one of the organization's user account")

	_Signing in using one of the organization's user account_

1. Show that you are loggued as the organization's user. 

	![Showing that you are logged as the organization's user](images/showing-the-organization-user-logged.png?raw=true "Showing that you are logged as the organization's user")

	_Showing that you are logged as the organization's user_

1. Close the browser

<a name="segment2" />
### Running the organization's GeekQuiz ###

1. Open the **GeekQuiz.sln** solution located under **source\end-segment2**.

1. **CTRL+F5** to run the web site.

1.	Sign in using a user account for your organization (ex. "user@mydomainname.onmicrosoft.com").

	![Signing in using one of the organization's user account](images/logging-in-with-an-organization-user.png?raw=true "Signing in using one of the organization's user account")

	_Signing in using one of the organization's user account_

1. Show that you are loggued as the organization's user. 

	![Showing that you are logged as the organization's user](images/showing-the-geekquiz-with-waad.png?raw=true "Showing that you are logged as the organization's user")

	_Showing that you are logged as the organization's user_

---

<a name="summary" />
## Summary ##

(TODO: Insert a summary text here. For example:)  
By completing this demo lab you have learned how to:

 * (TODO: Insert outcome 1 here)
 * (TODO: Insert outcome 2 here)
 * (TODO: Insert outcome 3 here)

---