{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# Managing {{site.data.keyword.Bluemix_notm}}
{: #mng}

*Last updated: 15 October 2015*

Use the Admin Console to manage resources, monitor usage, administer user permissions, and view security
reports, logs, status, and upgrade notifications for your {{site.data.keyword.Bluemix}} Local or Dedicated environment. 
{:shortdesc}

## Accessing the Admin Console
{: #oc_access}

You can access the Admin Console by entering the following URL:

`https://opsconsole.<subdomain>.bluemix.net/`. 

<dl>
<dt><strong>&lt;subdomain&gt;</strong></dt>
<dd>This value is the name of your local or dedicated instance. The subdomain name for your {{site.data.keyword.Bluemix}} instance was
assigned during onboarding.</dd>
</dl>

## Viewing system information
{: #oc_system}

Use the Admin Console to monitor your system information. 

To view system information, click **ADMINISTRATION &gt; SYSTEM INFORMATION**.

You can expand and view various sections about pending updates, general system information, and
LDAP configuration details. 

* In the Updates section, you can view any pending
updates that require action on your part. You can also easily track your updates using the calendar
link to import your scheduled updates to a calendar app. 

<ol>
<li>To take action for a specific update, complete the following steps: 
<ol type="a">
<li>Click <strong><em>Number</em> updates pending</strong> to view all pending
updates.</li>
<li>Select an update to take action or view the details of the update, which include the update
window, scheduled date, or disruption status.</li>
<li>Click <strong>SET UNAVAILABLE DATES</strong> to set specific days in the update window
that are not convenient for the update to be applied. If you set unavailable dates, IBM approves and
schedules your update based on your selections. You receive a notification when the update is
approved and scheduled.</li>
<li>Click <strong>APPROVE</strong> to approve the update, if you do not have any unavailable
dates. If you approve, the update is applied during the scheduled update window. IBM sends a
notification when the update deployment starts and ends.</li>
</ol>
</li>
<li>To import your scheduled updates to a calendar app, complete the following steps:
<ol type="a">
<li>Open your calendar app.</li>
<li>Import the updates calendar using the Calendar URL.</li>
<li>Enter your credentials.</li>
<li>View your scheduled updates.</li>
</ol>
</li>
</ol>

* In the General Information section, you can view the following information: 
    * Basic information about the {{site.data.keyword.Bluemix_notm}} build.
    * API information including the version, URL, region, and a link to the CLI documentation.
    * Shared domain information about your system and service.
    * Statistics about the total number of applications, users, and organizations.
* In the LDAP Configuration Details section, you can select the LDAP
server, and view information about user and group mappings. If you are using {{site.data.keyword.IBM}} WebID, it is indicated in the LDAP Configuration
Details section. 

## Viewing usage information
{: #oc_resource}

Use the Admin Console to monitor resource and network usage. 

To view resource information, click **ADMINISTRATION &gt; USAGE**.

In the Resource Monitoring section, you can view the following
information:

* Resource usage information, such as how many GB of memory and how many GB of disk space are
used. You can view the CPU usage averaged across all droplet execution agents (DEAs). Click the
**CPU** tile, and you can see the CPU usage for each DEA. The DEA with the
highest usage is listed first, and each is identified by their job and IP address. The CPU usage is
separated into three categories that include amount of CPU spent in system processes, amount of CPU
spent in user processes, and amount of CPU spent in waiting processes.
* Network usage information for bandwidth in and bandwidth out, over the past day, week, or month.
The data that is displayed is based on the sum of in and out traffic for both public and private
networks.
* Average response time for {{site.data.keyword.Bluemix_notm}} over the past 10 minutes, hour, and day.
* Average transactions per second for 
{{site.data.keyword.Bluemix_notm}} over the past 10
minutes, hour, and day.

## Viewing reports
{: #oc_report}

You can view security reports and logs, such as DataPower&trade;, firewall, and login audit, for
your {{site.data.keyword.Bluemix_notm}} instance.

To view reports and logs, click **ADMINISTRATION &gt; REPORTS AND LOGS**.

Select from the following options:

* You can select start and end dates from the fields to filter which reports and logs are
displayed.
* You can expand and view various reports from the left navigation pane.
* You can search within your collection of reports and logs. The search applies to report
names as well as text content that is contained within the reports and logs. You can also choose to
filter your search by **Administration Events**, **DataPower Reports**, **Firewall**, and **Login Audit**.
* When displaying a report or log, you can click the ![Download](images/icon_download.png)
icon at the upper right of the report to download it.

## Viewing status
{: #oc_status}

You can monitor status for your {{site.data.keyword.Bluemix_notm}} instance through the Admin
Console. You can also subscribe to an RSS feed for notifications so that you don't have to check for them. 

To view status for your {{site.data.keyword.Bluemix_notm}} instance, complete the following steps:

1. In the Admin Console in the upper-right corner, click the
**Profile Settings** icon.

2. Then, click **Status**.

The System Status page displays. The left pane displays the status
of your runtimes and services across regions and your {{site.data.keyword.Bluemix_notm}} instance. The right pane shows notifications.

3. If you configured your browser for RSS feeds, you can subscribe to an RSS feed of the
notifications. Locate the ![RSS](images/icon_RSS.png) icon to the right of **UPDATES** at the top left of the notifications list, and select one of the following actions: 

* Drag the ![RSS](images/icon_RSS.png) icon into your RSS reader.
* Right-click the RSS icon, select **Copy link address**, and paste the URL
into your RSS reader. 

4. Filter which notifications are displayed. Click **FILTER** at the top right
of the notifications list. Then, you can search and narrow the list of notifications by typing a
word that you would expect to find in a notification, for example "maintenance". Or, you can
click to select which notifications to display by **Type**,
**Region**, **Category**, **Start date**, or **End date**. 

## Managing your Catalog
{: #oc_catalog}

You can manage which {{site.data.keyword.Bluemix_notm}} services and starters are visible to users in the {{site.data.keyword.Bluemix_notm}} Catalog.

To use the Admin Console to manage the Catalog,
click **ADMINISTRATION &gt; CATALOG MANAGEMENT**.

Select a service or starter tile to edit the service or starter plan visibility. To edit the
visibility, select from the following options:
* To show the hidden service or starter so that it is visible to your users in the
Catalog, select **ENABLE ALL PLANS**.
* To hide the service or starter from your users in the {{site.data.keyword.Bluemix_notm}}
Catalog, select **DISABLE ALL PLANS**.
* To control the visibility of an individual plan, select the plan name, and then use the
drop-down menu to select **Enable for all organizations**, **Disable for
all organizations**, or **Enable plan for specific
organizations**.

## Administering organizations
{: #oc_organizations}

You can manage your organizations by creating and deleting organizations, adding managers to organizations, and monitoring quota usage.

To use the Admin Console to manage your organizations, click **ADMINISTRATION &gt; ORGANIZATION ADMINISTRATION**.

You can expand and view various sections. You can also review and manage the quota plans for
your organizations.

* To create a new organization and add managers, click <strong>CREATE ORGANIZATION</strong>. 
Enter a name for the organization, and then enter the name or email of the
person that you want to add as a manager. You can add more than one manager by entering and
selecting multiple names. Click <strong>CREATE ORGANIZATION</strong> to save your changes and
create the org. 
* In the Quota Monitoring section, you can expand the section and view
the following information:
    * Environment memory usage. This section details the memory usage for the full system environment.
	The chart provides information that includes used system memory, total system memory, quota that is
	used, and the total quota allocated. The following list of terms defines the types of memory usage
	that are displayed in the chart.
	<dl>
	<dt><strong>Used system memory</strong></dt>
	<dd>The physical memory that is used by your environment.</dd>
	<dt><strong>Total system memory</strong></dt>
	<dd>The total physical memory that is available to your environment.</dd>
	<dt><strong>Quota deployed</strong></dt>
	<dd>The sum of memory that is allocated for all deployed apps, across all organizations. The sum of
	the quota deployed can exceed the physical total system memory for your environment. For example, if
	you have a total system memory of 16 GB, and you allocate 4 GB of memory each for a total of five
	different organizations, the total quota exceeds the total system memory that has been allocated to
	you for all organizations. However, in many cases, the organizations might not use the total quota
	that is allocated individually to each organization. In addition, all organizations might not use
	their total quota allocation of memory all at the same time. </dd>
	<dt><strong>Total quota</strong></dt>
	<dd>The total memory that is allocated across all organizations.</dd>
	</dl>
	* Organization memory usage. This section details the memory usage at an organization level. You
	can view the total quota allowance and the quota that is deployed for each organization. The chart
	provides information that is listed by highest memory usage per organization, and the organization
	that uses the largest amount of memory, by default, is listed first. You can sort by
	** Highest Memory Usage** and **Excess Memory Allocation**.
	<dl>
	<dt><strong>Highest Memory Usage</strong></dt>
	<dd>Use this option to identify the org using the greatest amount of memory. Sort by highest memory
	usage to identify the organizations that are using the most amount of memory. The list is sorted by
	quota deployed. </dd>
	<dt><strong>Excess Memory Allocation</strong></dt>
	<dd>Use this option to identify organizations that have a quota plan that is larger than needed.
	Sort by excess memory usage to identify organizations that are using the lowest amount of memory for
	the quota that has been allocated for the org. </dd>
	</dl>
* To change the quota plan for an organization, click the bar in the chart for the
organization that you want to edit in the Organization memory usage section, or select the name of
the org from the Organization List section. On the Edit
Organization page, you can change the quota plan, change the name of the org, and add or
remove managers. If you select a quota plan that is not sufficient for the current usage for the
organization, you receive a message. To save any changes that you made on the Edit
Organization page, click **SAVE**.
* In the Organization List section, you can view all organizations in the
{{site.data.keyword.Bluemix_notm}} environment.
	* To delete the organization, click ![Delete](images/icon_trash.png) in the Actions column.
	* To view and edit the quota plan for an organization, click the name for the organization in the
	list.
	* To edit the name of the org and add or remove managers, click the name for the organization in
	the list.

## Managing users and permissions
{: #oc_useradmin}
You can add users to your {{site.data.keyword.Bluemix_notm}} instance from your company's user registry through LDAP. You can add users singly or in
groups, and view user permissions. If you are assigned `admin` permission, you
can also set and manage permissions for other users.

To use the Admin Console to manage users, click **ADMINISTRATION &gt; USER ADMINISTRATION**.

The User Administration page displays all users for the local or dedicated instance.
Permissions for each user are displayed. Permissions can be the following: None,
`Admin`, `Catalog`, `Login`,
`Reports`, and `Users`. Permissions can be enabled, or the
user can be given `view` or `write` ability for that
permission, as represented by icons. See [Permissions](#permissions) for descriptions
of each type and explanation of the icons. 

Choose from the following options:
* Locate users.You can locate users in the table by using the **Search**
field at the top.
* Add users. If you have `admin` permission or
`users` permission with `write` ability, you can add users. To
add a user or group of users, click **ADD SINGLE USER** or **ADD USER
GROUP**. In the **Search** field, type a user name or group name to
search, and select the organization to add the user or user group to from the
**Org** list. When you find the user or group that you want to add, click the
user name, then click **ADD USER** or **ADD USERS** to add.
Groups of more than 50 users are added through a background batch job. When the add operation
is successful, the user or group is added to the table for you to view and search. When users are
added, they have no assigned permissions.
* Edit permissions and organizations. If you have `admin` permission,
you can edit permissions and organizations for other users. To edit permissions, locate the user and
click the user name. To enable or disable permissions, select from the following options in the
window that opens:
	* Select **On** from the list to enable a permission.
	* Select **Read** from the list to allow the user to have `view` (read-only) ability for that permission, or **Write**
	to allow `write` (edit, or add and remove) ability for that permission.
	* Select **Off** to disable the permission.
To edit organizations, select from the following options:
	* Add the user to an organization by using the search field to locate an organization, clicking to
	select from the options, and clicking **ADD**.
	* Remove a user from an organization by clicking the ![Remove, represented by a minus sign](images/icon_remove.png) icon.
When finished, click **SAVE**.
* Remove users. If you have `admin` permission or
`users` permission with `write` ability, you can remove users.
To remove a user, locate the user and click the ![Delete](images/icon_trash.png) icon and then **Remove**.

### Permissions
{: #permissions}

Users can be assigned the following permissions:

| **User permission** | **Description** |       
|-----------------|-------------------|
| Admin | Users with `admin` permission are allowed to edit permissions for other users. | 
| Catalog | Users with `catalog` permission can be assigned the ability to `view` or `write` (modify) which services are available in the local or dedicated instance. |  
| Login | Users with `login` permission are allowed to log in to the Admin Console. Without this permission, users can't log in. |
| Reports | Users with `reports` permission can be assigned the ability to `view` or `write` (modify) security reports. |
| Users | Users with `users` permission can be assigned the ability to `view` the list of users or `write` (add or remove) users. This permission doesn't allow you to set permissions for other users.|

*Table 1. Permissions*

Permissions can be enabled, or the user can be given `view` or
`write` ability for that permission, as represented by the following icons:

* The ![Enabled, represented by a check mark](images/icon_enabled.png) icon beside a permission means that it is enabled.
* The ![View, represented by an eye](images/icon_read.png) icon means that the user has `view` (read-only) ability for that permission.
* The ![Write, represented by a pencil](images/icon_write.png) icon means that the user has `write` (edit, add, or remove) ability for that permission.

## Managing users with the Admin REST API
{: #usingadminapi}

You can use the `Admin` REST API to add and remove users for your
{{site.data.keyword.Bluemix_notm}} instance.
The `Admin` REST API endpoints and JSON responses are provided on an experimental
basis to enable basic operations from a command line. The endpoints and URLs in the examples in this
information might change or might be discontinued at short notice.

The following tools are prerequisites for using the examples that follow. You can choose to
use other tools as well.
* cURL, to enter REST API requests as commands. cURL is a free utility that you can use to send
HTTP requests to a server and receive the server responses through a command-line interface. You can
download cURL from the [cURL Download site](http://curl.haxx.se/download.html){: new_window}.
* Python, to use the Python pretty-print JSON tool. This optional tool takes the JSON text as
input and provides easy-to-read output. You can download Python from the [Python Downloads site](https://www.python.org/downloads){: new_window}.

### Logging in to the Admin Console

Before you can run any `Admin` API requests, you must log in to the
Admin Console. If you have `admin` permission or `users`
permission with `write` ability, you can add or remove users. You must have
`admin` permission to edit other users' permissions.

To log in to the Admin Console, you can use basic access authentication on the
`https://<your_host>.ibm.com/login` endpoint. The server returns a cookie with your
session. You use that cookie for all operations with the Admin Console.

**Note:** The session becomes invalid if not used for a few hours.

To log in to the Admin Console, run the following command:

`curl --user <user_id>:<password> -c ./cookies.txt --header "Accept: application/json" https://<your_host>.ibm.com/login | python -m json.tool`
{: codeblock}

<dl class="parml">

<dt class="pt dlterm">--user <em>user_id</em>:<em>password</em></dt>
<dd class="pd">Accepts the user ID and password and sends a Basic Authorization header.</dd>


<dt class="pt dlterm">-c <em>filename</em></dt>
<dd class="pd">Stores the specified user ID and password as a cookie in the specified file.</dd>


<dt class="pt dlterm">--header</dt>
<dd class="pd">Sends an Accept header.</dd>

</dl>

The following example shows output from this
command:
```
{
    "message": "Logged in",
    "name": {
        "familyName": "*last_name*",
        "givenName": "*first_name*"
    }
}
```
{: screen}

### Listing organizations
{: #listingorg}

When you add a user, you must specify an organization. You can use the
`Admin` REST API to list all organizations. You must have
`users` permission with `read` ability to list
organizations.To list all organizations, run the following command:

`curl -b ./cookies.txt https://<your_host>.ibm.com/codi/v1/organizations | python -m json.tool`
{: codeblock}

<dl class="parml">

<dt class="pt dlterm">-b <em>filename</em></dt>
<dd class="pd">Passes the user ID and password that was previously stored with the <samp class="ph codeph">-c</samp>
option in the file to the HTTP server as a cookie.</dd>

</dl>

For each organization, the results include the following information: 
* `"guid"`, GUID of the organization
* `"name"`, name of the organization

The following example shows output from this command:
``` 
{
     "resources": [
         {
             "guid": "05af098d-d476-4fb0-8b87-a84350e72af3",
             "name": "org-1"
         },
         {
             "guid": "5129a5a8-37c2-4ee4-a9b2-bebae3531db5",
             "name": "org-2"
         },
 
		 		 ....
		 		 
		 ],
		 "total_results": 284
}
```
{: screen}

### Listing users
{: #listingusr}

You can determine whether a user was already added to your 
{{site.data.keyword.Bluemix_notm}} environment by
using the `Admin` REST API to list registered users. You must have
`users` permission with `read` ability to list registered
users.To list all users, run the following command:

`curl -b ./cookies.txt https://<your_host>.ibm.com/codi/v1/users | python -m json.tool`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">-b <em>filename</em></dt>
<dd class="pd">Passes the user ID and password that was previously stored with the <samp class="ph codeph">-c</samp>
option in the file to the HTTP server as a cookie.</dd>
</dl>

For each registered user, the results include the following information: 
* `"first_name"` (given name) and `"last_name"` (surname)
* `"user_id"`, user ID and email address
* `"guid"`, GUID of the organization.
* `"permissions"` that are assigned to the user for the Admin Console.

The following example shows output from this command:

```
{
    "next_url": "/codi/v1/users?results_per_page=100&amp;page=2",
    "prev_url": "",
    "resources": [
        {
            "active": true,
            "created_at": "2015-04-08T17:38:51.788Z",
            "created_by": "",
            "first_name": "some first name",
            "guid": "5d5268cf-39c0-48d3-96ae-7afe928e5dd7",
            "last_name": "some last name",
            "permissions": [
                {
                    "display": "ops.admin"
                },
                {
                    "display": "ops.catalog.write"
                },
                {
                    "display": "ops.reports.write"
                },
                {
                    "display": "ops.catalog.read"
                },
                {
                    "display": "ops.users.write"
                },
                {
                    "display": "ops.reports.read"
                },
                {
                    "display": "ops.login"
                },
                {
                    "display": "ops.users.read"
                }
            ],
            "user_id": "someid@us.ibm.com"
        },
		 		 ...
		 		 
		 		 
     }
    ],
    "total_pages": 395,
    "total_results": 39421
}

```
{: screen}

### Adding a user

You can use the `Admin` REST API to add users to the 
{{site.data.keyword.Bluemix_notm}} instance. You must
have `users` permission with `write` ability to add
users.

You can add one user or a list of users. You can add users to a single
organization, or to multiple organizations.-->To
add a user, you must provide the following information:

* First name (given name) and last name (surname) of the user. Provide the
`"first_name"` and `"last_name"` from [Listing users](index.html#listingusr).
* Email address and user ID: Provide the `"user_id"` from [Listing users](index.html#listingusr) for both the email address and the user ID.
* `"guid"`. Provide the GUID of the organization from [Listing organizations](index.html#listingorg).

You provide the information in a JSON file.

`curl -b ./cookies.txt https://<your_host>.ibm.com/codi/v1/users | python -m json.tool`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">-b <em>filename</em></dt>
<dd class="pd">Passes the user ID and password that was previously stored with the <samp class="ph codeph">-c</samp>
option in the file to the HTTP server as a cookie.</dd>
</dl>

<ol>
<li>Create a JSON file that contains the information in a proper JSON format. 
<p>For example, create a file that is named `user.json` that has the
following content:</p>
<code>
{
    "members": [
        {
            "emails": [
                "some_user_id@domain.com"
            ],
            "first_name": "Some_first_name",
            "last_name": "Some_last_name",
            "user_id": "some_user_id@domain.com"
        }
    ],
    "organization_roles": [
        {
            "id": "7a891f9c-e4e7-46c7-8b4e-dffaa7eb3bcd"
        }
    ]
}
</code><br/><br/>
</li>
<li>Post the content of the JSON file to the user's endpoint by running the following
command:<br/><br/>
<code>
curl -v -b ./cookies.txt -X POST -H "Content-Type: application/json" -d @./user.json https://<your_host>.ibm.com/codi/v1/users
</code>
</li>
</ol>

<dl class="parml">

<dt class="pt dlterm">-v </dt>
<dd class="pd">Specifies verbose output.</dd>


<dt class="pt dlterm">-X POST</dt>
<dd class="pd">Specifies a POST request, overriding the default GET request.</dd>


<dt class="pt dlterm">-H "Content-Type: application/json"</dt>
<dd class="pd">Specifies the content-type header, which in this case is JSON.</dd>


<dt class="pt dlterm">-d *data*</dt>
<dd class="pd">Specifies the data, in this case the file `user.json`, to be sent in POST
request to the HTTP server.</dd>

</dl>



The following example shows output from this
command:

``` 
* Connected to localhost (127.0.0.1) port 3000 (#0)
 > POST /codi/v1/users HTTP/1.1
 > User-Agent: curl/7.37.1
 > Host: localhost:3000
 > Accept: */*
 > Cookie: opsConsole.sid=s%3AHLcwKGumyEb3IxREmikDOG3ATKD5xYMe.jfjWAa1tJC0rGghpeV8RPHqE2JaFVL4ZFIJbQpSC%2FAI
 > Content-Type: application/json
 > Content-Length: 333
 > 
 * upload completely sent off: 333 out of 333 bytes
 &lt; HTTP/1.1 201 Created
 &lt; x-powered-by: Express
 &lt; vary: X-HTTP-Method-Override
 &lt; content-type: application/json
 &lt; date: Wed, 22 Apr 2015 19:32:54 GMT
 &lt; connection: close
 &lt; transfer-encoding: chunked
 &lt; X-Time_Check: Proxy Time: 5612 msec
 ``` 
{: screen}

### Removing a user

You can use the `Admin` REST API to remove users from the 
{{site.data.keyword.Bluemix_notm}} instance. You must
have `users` permission with `write` ability to remove users.

To remove a user, you must provide the user ID of the user. Run the following command:

`curl -v -b ./cookies.txt -X DELETE https://<your_host>.ibm.com/codi/v1/users?user_id=<some_user_id@domain.com>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">-X DELETE</dt>
<dd class="pd">Specifies a DELETE request.</dd>
</dl>

The following example shows output from this
command:

```
 * connect to ::1 port 3000 failed: Connection refused
 *   Trying 127.0.0.1...
 * Connected to localhost (127.0.0.1) port 3000 (#0)
 &gt; DELETE /codi/v1/users?user_id=exampleuser@domain.com HTTP/1.1
 &gt; User-Agent: curl/7.37.1
 &gt; Host: localhost:3000
 &gt; Accept: */*
 &gt; Cookie: opsConsole.sid=s%3AHLcwKGumyEb3IxREmikDOG3ATKD5xYMe.jfjWAa1tJC0rGghpeV8RPHqE2JaFVL4ZFIJbQpSC%2FAI
 &gt; 
 &lt; HTTP/1.1 201 Created
 &lt; x-powered-by: Express
 &lt; content-type: application/json
 &lt; date: Wed, 22 Apr 2015 21:01:09 GMT
 &lt; connection: close
 &lt; transfer-encoding: chunked
 &lt; X-Time_Check: Proxy Time: 1922 msec
 &lt; 
 ``` 
{: screen}

## Managing users with the cf CLI
{: #usingadmincli}

You can manage users for your 
{{site.data.keyword.Bluemix_notm}} environment by
using the Cloud Foundry command line interface with the 
{{site.data.keyword.Bluemix_notm}} Admin CLI plug-in. For
example, you can add users from an LDAP registry.

Before you begin, install the cf command line interface. The 
{{site.data.keyword.Bluemix_notm}} Admin CLI plug-in
requires cf version 6.11.2 or later. [Download Cloud Foundry command line interface](https://github.com/cloudfoundry/cli/releases){: new_window}

**Restriction:** The Cloud Foundry command line interface is not supported by
Cygwin. Use the Cloud Foundry command line interface in a command line window other than the Cygwin
command line window.

### Adding the {{site.data.keyword.Bluemix_notm}} Admin CLI plug-in

After the cf command line interface is installed, you can add the 
{{site.data.keyword.Bluemix_notm}} admin CLI
plug-in.

Complete the following steps to add the repository and install the plug-in: 

<ol>
<li>To add the {{site.data.keyword.Bluemix_notm}} admin plug-in repository, run the following command:<br/><br/>
<code>
cf add-plugin-repo BluemixAdmin https://opsconsole.<subdomain>;.bluemix.net/cli
</code><br/><br/>
<dl class="parml">
<dt class="pt dlterm">&lt;subdomain&gt;</dt>
<dd class="pd">Subdomain of the URL for your {{site.data.keyword.Bluemix_notm}} instance.</dd>
</dl>
</li>
<li>To install the {{site.data.keyword.Bluemix_notm}} Admin CLI plug-in, run the following command:<br/><br/>
<code>
cf install-plugin bluemix-admin-cli -r BluemixAdmin
</code>
</li>
</ol>

### Using the {{site.data.keyword.Bluemix_notm}} Admin CLI plug-in

You can use the {{site.data.keyword.Bluemix_notm}} Admin CLI plug-in to add or remove users, assign or unassign users from orgs, and to perform other management tasks. To see a list of commands, run the following
command:

`cf plugins`
{: codeblock}

For additional help for a command, use the `--help` option.

#### Connecting and logging in to {{site.data.keyword.Bluemix_notm}}

Before you can use the Admin CLI plug-in to manage users, you must connect and log in, if
you are not already.

<ol>
<li>To connect to the {{site.data.keyword.Bluemix_notm}}> API endpoint, run the following command:<br/><br/>
<code>
cf api https://api.<subdomain>.bluemix.net
</code>
<dl class="parml">
<dt class="pt dlterm">&lt;subdomain&gt;</dt>
<dd class="pd">Subdomain of the URL for your {{site.data.keyword.Bluemix_notm}} instance.</dd>
</dl>
<p>You can check the Admin Console Resources and Information page for the
correct URL. The URL is shown in the API Information section in the **API URL**
field.</p>
</li>
<li>Log in to {{site.data.keyword.Bluemix_notm}} with the following command:<br/><br/>
<code>
cf login
</code>
</li>
</ol>

#### Adding a user

You can add a user to your 
{{site.data.keyword.Bluemix_notm}} environment from
an LDAP registry. Enter the following command: 

`cf bluemix-admin-add-user <user_name> <organization>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;user_name&gt;</dt>
<dd class="pd">The name of the user in the LDAP registry.</dd>
<dt class="pt dlterm">&lt;organization&gt;</dt>
<dd class="pd">The name or GUID of the {{site.data.keyword.Bluemix_notm}} org to add the user to.</dd>
</dl>

**Tip:** You can also use **baau** as an alias for the longer
**bluemix-admin-add-user** command name.

#### Removing a user

You can remove a user from your 
{{site.data.keyword.Bluemix_notm}} environment by
entering the following command: 

`cf bluemix-admin-remove-user <user_name>`
{: codeblock}

<dl class="parml">

<dt class="pt dlterm">&lt;user_name&gt;</dt>
<dd class="pd">The name of the user in {{site.data.keyword.Bluemix_notm}}.</dd>

</dl>

**Tip:** You can also use **baru** as an alias for the longer
**bluemix-admin-remove-user** command name.

#### Adding and deleting an organization

You can add and delete an organization.

* To add an organization, enter the following command:

`cf Bluemix-admin-create-organization <organization> <manager>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;organization&gt;</dt>
<dd class="pd">The name or GUID of the {{site.data.keyword.Bluemix_notm}} org to add.</dd>
<dt class="pt dlterm">&lt;manager&gt;</dt>
<dd class="pd">The user name of the manager for the org.</dd>
</dl>

**Tip:** You can also use **baco** as an alias for the longer
**bluemix-admin-create-organization** command name.

* To delete an organization, enter the following command:

`cf Bluemix-admin-delete-organization <organization>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;organization&gt;</dt>
<dd class="pd">The name or GUID of the {{site.data.keyword.Bluemix_notm}} org to delete.</dd>
</dl>

**Tip:** You can also use **bado** as an alias for the longer
**bluemix-admin-create-organization** command name.

#### Assigning a user to an organization

You can assign a user in your 
{{site.data.keyword.Bluemix_notm}} environment to a
particular organization. Enter the following command: 

`cf bluemix-admin-set-org <user_name> <organization> [<role>]`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;user_name&gt;</dt>
<dd class="pd">The name of the user in {{site.data.keyword.Bluemix_notm}}.</dd>
<dt class="pt dlterm">&lt;organization&gt;</dt>
<dd class="pd">The name or GUID of the {{site.data.keyword.Bluemix_notm}} org to assign the user to.</dd>
<dt class="pt dlterm">&lt;role&gt;</dt>
<dd class="pd">See [Roles](#roles) for 
{{site.data.keyword.Bluemix_notm}} user roles and
descriptions.</dd>
</dl>

**Tip:** You can also use **baso** as an alias for the longer
**bluemix-admin-set-org** command name.

#### Unassigning a user from an organization

You can unassign a user in your 
{{site.data.keyword.Bluemix_notm}} environment from a
particular organization. Enter the following command: 

`cf bluemix-admin-unset-org <user_name> <organization> [<role>]`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;user_name&gt;</dt>
<dd class="pd">The name of the user in {{site.data.keyword.Bluemix_notm}}.</dd>
<dt class="pt dlterm">&lt;organization&gt;</dt>
<dd class="pd">The name or GUID of the {{site.data.keyword.Bluemix_notm}} org to assign the user to.</dd>
<dt class="pt dlterm">&lt;role&gt;</dt>
<dd class="pd">See [Roles](#roles) for 
{{site.data.keyword.Bluemix_notm}} user roles and
descriptions.</dd>
</dl>

**Tip:** You can also use **bauo** as an alias for the longer
**bluemix-admin-unset-org** command name.

### Roles

<dl class="parml">
<dt class="pt dlterm">OrgManager</dt>
<dd class="pd">Organization manager. An org manager has authority to do the following actions:
<ul>
<li>Create or delete spaces within the organization.</li>
<li>Invite users to the organization and manage users.</li>
<li>Manage domains of the organization.</li>
</ul>
</dd>
<dt class="pt dlterm">BillingManager</dt>
<dd class="pd">Billing manager. A billing manager can view runtime and service usage information for the
organization.</dd>
<dt class="pt dlterm">OrgAuditor</dt>
<dd class="pd">Organization auditor. An organization auditor can view application and service content in the
space.</dd>
</dl>

### Setting a quota for an organization

You can set the usage quota for a particular organization. 

`cf bluemix-admin-set-quota <organization> <plan>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;organization&gt;</dt>
<dd class="pd">The name or GUID of the {{site.data.keyword.Bluemix_notm}} org to set the quota for.</dd>
<dt class="pt dlterm">&lt;plan&gt;</dt>
<dd class="pd">The quota plan for an organization.</dd>
</dl>

**Tip:** You can also use **basq** as an alias for the longer
**bluemix-admin-set-quota** command name.

### Adding, deleting, and retrieving reports

You can add, delete, and retrieve security reports. 
* To add a report, enter the following command:

`cf bluemix-admin-add-report <category> <date> <PDF|TXT|LOG> <RTF>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;category&gt;</dt>
<dd class="pd">The category for the report. If there is a space in the name, use quotation marks around the
name.</dd>
<dt class="pt dlterm">&lt;date&gt;</dt>
<dd class="pd">The report date in the format <samp class="ph codeph">YYYYMMDD</samp>.</dd>
<dt class="pt dlterm">&lt;PDF|TXT|LOG&gt;</dt>
<dd class="pd">The path for the report PDF, text file, or log file to upload.</dd>
<dt class="pt dlterm">&lt;RTF&gt;</dt>
<dd class="pd">An option to include a Rich Text Format (RTF) version of the PDF. This option applies only if
you included a path to the report PDF. The RTF version is used for indexing and searching.</dd>
</dl>

**Tip:** You can also use **baar** as an alias for the longer
**bluemix-admin-add-report** command name.

* To delete a report, enter the following command:

`cf bluemix-admin-delete-report <category> <date> <name>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;category&gt;</dt>
<dd class="pd">The category for the report. If there is a space in the name, use quotation marks around the
name.</dd>
<dt class="pt dlterm">&lt;date&gt;</dt>
<dd class="pd">The report date in the format <samp class="ph codeph">YYYYMMDD</samp>.</dd>
<dt class="pt dlterm">&lt;name&gt;</dt>
<dd class="pd">The name of the report.</dd>
</dl>

**Tip:** You can also use **badr** as an alias for the longer
**bluemix-admin-delete-report** command name.

* To retrieve a report, enter the following command:

`cf bluemix-admin-retrieve-report <category> <date> <name>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;category&gt;</dt>
<dd class="pd">The category for the report. If there is a space in the name, use quotation marks around the
name.</dd>
<dt class="pt dlterm">&lt;date&gt;</dt>
<dd class="pd">The report date in the format <samp class="ph codeph">YYYYMMDD</samp>.</dd>
<dt class="pt dlterm">&lt;name&gt;</dt>
<dd class="pd">The name of the report.</dd>
</dl>

**Tip:** You can also use **barr** as an alias for the longer **bluemix-admin-retrieve-report** command name.

### Enabling and disabling services for all organizations

You can enable or disable a service from being displayed in the 
{{site.data.keyword.Bluemix_notm}} Catalog for all organizations.

* To enable a service to be visible in the 
{{site.data.keyword.Bluemix_notm}} Catalog for all
organizations, enter the following command:

`cf bluemix-admin-enable-service-plan <plan_identifier>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;plan_identifier&gt;</dt>
<dd class="pd">The name or GUID of the service that you want to enable. If you enter a non-unique service name,
you are prompted with service plans to choose from.</dd>
</dl>

**Tip:** You can also use **baesp** as an alias for the longer
**bluemix-admin-enable-service-plan** command name.

* To disable a service from being visible in the 
{{site.data.keyword.Bluemix_notm}} Catalog for all
organizations, enter the following command:

`cf bluemix-admin-disable-service-plan <plan_identifier>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;plan_identifier&gt;</dt>
<dd class="pd">The name or GUID of the service that you want to disable. If you enter a non-unique service
name, you are prompted with service plans to choose from.</dd>
</dl>

**Tip:** You can also use **badsp** as an alias for the longer
**bluemix-admin-disable-service-plan** command name.

### Adding, removing, and editing service visibility for organizations

You can add or remove an organization from the list of organizations that can see a
specific service in the {{site.data.keyword.Bluemix_notm}} Catalog. You can also edit and replace the list of services that specific
organizations can see in the {{site.data.keyword.Bluemix_notm}} Catalog. 

* To allow an organization to view a specific service in the 
{{site.data.keyword.Bluemix_notm}} Catalog, enter the
following command:

`cf bluemix-admin-add-service-plan-visibility <plan_identifier> <organization>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;plan_identifier&gt;</dt>
<dd class="pd">The name or GUID of the service that you want to add visibility for. If you enter a non-unique
service name, you are prompted with service plans to choose from.</dd>
<dt class="pt dlterm">&lt;organization&gt;</dt>
<dd class="pd">The name or GUID of the {{site.data.keyword.Bluemix_notm}} org to add to the service's visibility list.</dd>
</dl>

**Tip:** You can also use **baaspv** as an alias for the longer
**bluemix-admin-add-service-plan-visibility** command name.

* To remove the visibility of a service in the 
{{site.data.keyword.Bluemix_notm}} Catalog for an
organization, enter the following command:

`cf bluemix-admin-remove-service-plan-visibility <plan_identifier> <organization>`
{: codeblock}

<dl class="parml">
<dt class="pt dlterm">&lt;plan_identifier&gt;</dt>
<dd class="pd">The name or GUID of the service that you want to remove visibility for. If you enter a
non-unique service name, you are prompted with service plans to choose from.</dd>
<dt class="pt dlterm">&lt;organization&gt;</dt>
<dd class="pd">The name or GUID of the {{site.data.keyword.Bluemix_notm}} org to remove from the service's visibility list.</dd>
</dl>

**Tip:** You can also use **barspv** as an alias for the longer
**bluemix-admin-remove-service-plan-visibility** command name.

* To replace all existing visible services for an organization or multiple organizations, use the
following command:

`cf bluemix-admin-edit-service-plan-visibilities <plan_identifier> <organization_1> <optional_organization_2>`
{: codeblock}

**Note:** This
command replaces existing visible services for the specified organizations with the service that you
specify in the command.

<dl class="parml">
<dt class="pt dlterm">&lt;plan_identifier&gt;</dt>
<dd class="pd">The name or GUID of the service that you want to make visible. If you enter a non-unique service
name, you are prompted with service plans to choose from.</dd>
<dt class="pt dlterm">&lt;organization&gt;</dt>
<dd class="pd">The name or GUID of the {{site.data.keyword.Bluemix_notm}} org to add visibility for. You can enable visibility of the service for more than
one organization by entering additional organization names or GUIDs in the command.</dd>
</dl>

**Tip:** You can also use **baespv** as an alias for the longer
**bluemix-admin-edit-service-plan-visibility** command name.
