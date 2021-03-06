### May 2015

#### Bug fixes
  - Updated nested addHosts to use variables passed (PR889)

#### Improvements
  - Added loading bar to top nav (PR893)
  - Added load and current for APC units (PR888)
  - Improved web installer (PR887)
  - Updated alerts status box (PR875)
  - Updated syslog page (PR862)
  - Added temperature polling for IBM Flexsystem (PR894)
  - Updated typeahead libraries and relevant forms (PR882)

### Apr 2015

####Bug fixes
  - Fixed ack of worse/better alerts (PR720)
  - Fixed ORIG_PATH_INFO warnings (PR727)
  - Added missing CPU id for Cisco SB (PR744)
  - Changed Processors table name to lower case in processors discovery (PR751)
  - Fixed alerts path issue (PR756, PR760)
  - Supress further port alerts when interface goes down (PR745)
  - Fixed login so redirects via 303 when POST data sent (PR775)
  - Fixed missing link to errored or ignored ports (PR787)
  - Updated alert log query for performance improvements (PR783)
  - Honour alert_rules.disabled field (PR784)
  - Stop page debug if user not logged in (PR785)
  - Added text filtering for new tables (PR797)
  - Fixed VMWare VM detection + hardware / serial support (PR799)
  - Fix links from /health/processor (PR810)
  - Hide divider if no plugins installed (PR811)
  - Added Nginx fix for using debug option (PR823)
  - Bug fixes for device groups SQL (PR840)
  - Fixed path issue when using rrdcached (PR839)
  - Fixed JS issues when deleting alert maps / poller groups / device groups (PR846,PR848,PR877)
  - Fixed links and popover for /health/metric=storage/ (PR847)
  - Fixed lots of user permission issues (PR855)
  - Fixed search ip / arp / mac pages (PR845)
  - Added missing charge icon (PR878)

####Improvements
  - New theme support added (light,dark and mono) (PR682,PR683,PR701)
  - Tables being converted to Jquery Bootgrid (PR693,PR706,PR716)
  - Detect Cisco ASA Hardware and OS Version (PR708)
  - Update LDAP support (PR707)
  - Updated APC powernet MIB (PR713)
  - Update to Foritgate support (PR709)
  - Added support for UBNT AirOS and AirFibre (PR721,PR730,PR731)
  - Added support device groups + alerts to be mapped to devices or groups (PR722)
  - Added basic Cambium support (PR738)
  - Added basic F5 support (PR670)
  - Shorten interface names on map (PR752)
  - Added PowerCode support (PR762)
  - Added Autodiscovery via OSPF (PR772)
  - Added visual graph of alert log (PR777, PR809)
  - Added Callback system to send anonymous stats (PR768)
  - More tables converted to use bootgrid (PR729, PR761)
  - New Global Cache to store common queries added (PR780)
  - Added proxy support for submitting stats (PR791)
  - Minor APC Polling change (PR800)
  - Updated to HP switch detection (PR802)
  - Added Datacom basic detection (PR816)
  - Updated Cisco detection (PR815)
  - Added CSV export system + ability to export ports (PR818)
  - Added basic detection for PacketLogic devices (PR773)
  - Added fallback support for IBM switches for Serial / Version (PR822)
  - Added Juniper Inventory support (PR825)
  - Sharpen graphs produced (PR826)
  - Updated map to show device overview graphs and port graphs (PR826)
  - Added hostname to API call for list_alerts (PR834)
  - Added ability to schedule maintenance (PR835,PR841)
  - Added ability to expand alert triggers for more details (PR857)
  - Added support for XTM/FBX Watchguard devices (PR849)
  - Updated Juniper MIBS and hardware rewrite (PR838)
  - Updated OpenBSD detection (PR860)
  - Added Macro support for alerting system (PR863)
  - Added support for tcp connections on rrdcached (PR866)
  - Added config option to enable / disable mouseover graphs (PR873)
  - General cleanup of files / folders permissions (PR874)
  - Added window size detection for map (PR884)
  - Added text to let users know refresh is disabled (PR883)

### Mar 2015

####Bug fixes
  - Updates to alert rules split (PR550)
  - Updated get_graphs() for API to resolve graph names (PR613)
  - Fixed use of REMOTE_ADDR to use X_FORWARDED_FOR if available (PR620)
  - Added yocto support from entPhySensorScale (PR632)
  - Eventlog search fixed (PR644)
  - Added missing OS discovery to default list (PR660)
  - Fixed logging issue when description of a port was removed (PR673)
  - Fixed logging issue when ports changed status (PR675)
  - Shortened interface names for graph display (PR676)

####Improvements
  - Visual updates to alert logs (PR541)
  - Added temperature support for APC AC units (PR545)
  - Added ability to pause and resume page refresh (PR557)
  - Added polling support for NXOS (PR562)
  - Added discovery support for 3Com switches (PR568)
  - Updated Comware support (PR583)
  - Added new logo (PR584)
  - Added dynamic removal of device data when removing device (PR592)
  - Updated alerting to use fifo (PR607)
  - Added distributed poller support (PR609 and PR610)
  - Added PowerConnect 55xx (PR635)
  - Added inventory API endpoint (PR640)
  - Added serial number detection for ASA firewalls (PR642)
  - Added missing MKTree library for inventory support (PR646)
  - Added support for exporting Alert logs to PDF (PR653)
  - Added basic Ubiquiti support (PR659)
  - Numerous docs update (PR662, PR663, PR677, PR694)
  - Added Polling information page (PR664)
  - Added HipChat notification support (PR669)
  - Implemented Jquery Bootgrid support (PR671)
  - Added new map to show xDP discovered links and devices (PR679 + PR680)

###Feb 2015

####Bug fixes
 - Removed header redirect causing page load delays (PR436)
 - Fixed stale alerting data (PR475)
 - Fixed api call for port stats to use device_id / hostname (PR478)
 - Work started on ensuring MySQL strict mode is supported (PR521)

####Improvements
 - Added support for Cisco Wireless Controllers (PR422)
 - Updated IRC Bot to support alerting system (PR434)
 - Added new message box to alert when a device hasn't polled for 15 minutes or more (PR435)
 - Added quick links on device list page to quickly access common pages (PR440)
 - Alerting docs updated to cover new features (PR446)
 - IBM NOS Support added (PR454)
 - Added basic Barracuda Loadbalancer support (PR456)
 - Small change to the search results to add port desc / alias (PR457)
 - Added Device sub menu to access devices category directly (PR465)
 - Added basic Ruckus Wireless support (PR466)
 - Added support for a demo user (PR471)
 - Many small visual updates
 - Added additional support for Cisco SB devices (PR487)
 - Added support to default home page for printing alerts (PR488)
 - Tidied up Alert menubar into sub menu (PR489)
 - Added historical alerts page (PR495)
 - Added battery charge monitoring for (PR519)
 - Added Slack support for alert system (PR525)
 - Added new debug for php / sql option to page footer (PR484)

###Jan 2015

####Bug fixes
 - Reverted chmod to make poller.php executable again (PR394)
 - Fixed duplicate port listing (PR396)
 - Fixed create bill from port page (PR404)
 - Fixed autodiscovery to use $config['mydomain'] correctly (PR423)
 - Fixed mute bug for alerts (PR428)

####Improvements
 - Updated login page visually (PR391)
 - Added Hikvision support (PR393)
 - Added ability to search for packages using unix agent (PR395)
 - Updated ifAlias support for varying distributions (PR398)
 - Updated visually Global Settings page (PR401)
 - Added missing default nginx graphs (PR403)
 - Updated check_mk_agent to latest git version (PR409)
 - Added support for recording process list with unix agent (PR410)
 - Added support for named/bind9/TinyDNS application using unix agent (PR413, PR416)
 - About page tidied up (PR414, PR425)
 - Updated progress bars to use bootstrap (PR42)
 - Updated install docs to cover CentOS7 (PR424)
 - Alerting system updated with more features (PR429, PR430)

###Dec 2014

####Bug fixes
 - Fixed Global Search box bootstrap (PR357)
 - Fixed display issues when calculating CDR in billing system (PR359)
 - Fixed API route order to resolve get_port_graphs working (PR364)

####Improvements
 - Added new API route to retrieve list of graphs for a device (PR355)
 - Added new API route to retrieve list of port for a device (PR356)
 - Added new API route to retrieve billing info (PR360)
 - Added alerting system (PR370, PR369, PR367)
 - Added dbSchema version to about page (PR377)
 - Added git log link to about page (PR378)
 - Added Two factor authentication (PR383)

###Nov 2014

####Bug fixes
 - Updated Alcatel-Lucent OmniSwitch detection (PR340)
 - Added fix for DLink port detection (PR347)
 - Fixed BGP session count (PR334)
 - Fixed errors with BGP polling and storing data in RRD (PR346)

####Improvements
 - Added option to clean old perf_times table entries (PR343)
 - Added nginx+php-fpm instructions (PR345)
 - Added BGP route to API (PR335)
 - Updated check_mk to new version + removed Observium branding (PR311)
 - Updated Edit SNMP settings page for device to only show relevant SNMP options (PR317)
 - Eventlog page now uses paged results (PR336)
 - Added new API route to show peering, transit and core graphs (PR349)
 - Added VyOS and EdgeOS detection (PR351 / PR352)
 - Documentation style and markdown updates (PR353)

###Oct 2014

####Bug fixes
 - Fixed displaying device image in device list (PR296)
 - Fixed placement of popups (PR297)
 - Updated authToken response code in API to 401 (PR310)
 - Removed trailing / from v0 part of API url (PR312)
 - Added correct response code for API call get_vlans (PR313)
 - Updated yearly graphs to fix year variable being passed (PR316)
 - Updated transport list to be generated from $config (PR318)
 - Moved addhost button on add host page as it was hidden (PR319)
 - Added stripslashes to hrdevice page (PR321)
 - Fixed web installer issue due to variable name change (PR325)
 - Updated disabled field in api tokens (PR327)
 - Fixed daily.sh not running from outside install directory (cron) (PR328)
 - Removed --no-edit from daily.php git pull (PR309)

####Improvements
 - Added ability to create api tokens (PR294)
 - Added icmp and poller graphs for devices (PR295)
 - Added urldecode/urlencode support for interface names in API (PR298)
 - Added new library to support on screen notifications (PR300)
 - Added authlog purge function and improved efficiency in clearing syslog table (PR301)
 - Updated addhost page to show relevant snmp options (PR303)
 - Added limit $config for front page boxes (PR305)
 - Updated http-auth adding user to check if user already exists (PR307)
 - Added names to all API routes (PR314)
 - Added route to call list of API endpoints (PR315)
 - Added options to $config to specify fping retry and timeout (PR323)
 - Added icmp / snnmp to device down alerts for debugging (PR324)
 - Added function to page results for large result pages (PR333)

###Sep 2014

####Bug fixes
 - Updated vtpversion check to fix vlan discovery issues (PR289)
 - Fixed mac address change false positives (PR292)

####Improvements
 - Hide snmp passwords on edit snmp form (PR290)
 - Updates to API (PR291)

###Aug 2014

####Bug fixes
 - Disk % not showing in health view (PR284)
 - Fixed layout issue for ports list (PR286)
 - Removed session regeneration (PR287)
 - Updated edit button on edit user screen (PR288)
  
####Improvements
 - Added email field for add user form (PR278)
 - V0 of API release (PR282)

###Jul 2014

####Bug fixes
 - Fixed RRD creation using MAX twice (PR266)
 - Fixed variables leaking in poller run (PR267)
 - Fixed links to health graphs (PR271)
 - Fixed install docs to remove duplicate snmpd on install (PR276)

####Improvements
 - Added support for Cisco ASA connection graphs (PR268)
 - Updated delete device page (PR270)

###Jun 2014

####Bug fixes
 - Fixed a couple of DB queries (PR222)
 - Fixes to make interface more mobile friendly (PR227)
 - Fixed link to device on overview apps page (PR228)
 - Fixed missing backticks on SQL queries (PR253 / PR254)
 - Fixed user permissions page (PR265)

####Improvements
 - Updated index page (PR224)
 - Updated global search visually (PR223)
 - Added contributors aggrement (PR225)
 - Added ability to update health values (PR226)
 - Tidied up search box on devices list page (PR229)
 - Updated port search box and port table list (PR230)
 - Removed some unused javascript libraries (PR231)
 - Updated year and column for vertical status summary (PR232)
 - Tidied up the delete user page (PR235)
 - Added snmp port to $config (PR237)
 - Added documentation for lighttpd (PR238)
 - Updated all device edit pages (PR239)
 - Added IPv6 only host support (PR241)
 - Added public status page (PR246)
 - Added validate_device_id function (PR257)
 - Added auto detect of install location (PR259)

###Mar 2014

####Bug fixes
 - Removed link to pdf in billing history (PR146)
 - librenms logs now saved in correct location (PR163)
 - Updated pfsense detection (PR182)
 - Fixed health page mini cpu (PR195)
 - Updated install docs to include php5-json (PR196)
 - Fixed Dlink interface names (PR200 / PR203)
 - Stop shortening IP in shorthost function (PR210)
 - Fixed status box overlapping (PR211)
 - Fixed top port overlay issue (PR212)
 - Updated docs and daily.sh to update DB schemas (PR215)
 - Updated hardware detection for RouterOS (PR217)
 - Restore _GET variables for logging in (PR218)

####Improvements
 - Updated inventory page to use bootstrap (PR141)
 - Updated mac / arp pages to use bootstrap (PR147)
 - Updated devices page to use bootstrap (PR149)
 - Updated delete host page to use bootstrap (PR151)
 - Updated print_error function to use bootstrap (PR153)
 - Updated install docs for Apache 2.3 > (PR161)
 - Upgraded PHPMailer (PR169)
 - Added send_mail function using PHPMailer (PR170)
 - Added new and awesome IRC Bot (PR171)
 - Added Gentoo detection and logo (PR174 / PR179)
 - Added Engenius detection (PR186)
 - Updated edit user to enable editing (PR187)
 - Added EAP600 engenius support (PR188)
 - Added Plugin system (PR189)
 - MySQL calls updated to use dbFacile (PR190)
 - Added support for Dlink devices (PR193)
 - Added Windows 2012 polling support (PR201)
 - Added purge options for syslog / eventlog (PR204)
 - Added BGP to global search box (PR205)

###Feb 2014

####Bug fixes
 - Set poller-wrapper.py to be executable (PR89)
 - Fix device/port down boxes (PR99)
 - Ports set to be ignored honoured for threshold alerts (PR104)
 - Added PasswordHash.php to adduser.php (PR119)
 - build-base.php update to run DB updates (PR128)

####Improvements
 - Added web based installer (PR75)
 - Updated login page design (PR78)
 - Ability to enable / disable topX boxes (PR100)
 - Added PHPPass support for MySQL auth logins (PR101)
 - Updated to Bootstrap 3.1 (PR106)
 - index.php tidied up (PR107)
 - Updated device overview page design (PR113)
 - Updated print_optionbar* to use bootstrap (PR115)
 - Updated device/port/services box to use bootstrap (PR117)
 - Updated eventlog / syslog to use bootstrap (PR132 / PR134)

###Jan 2014

####Bug fixes
 - Moved location redirect for logout (PR55)
 - Remove debug statements from process_syslog (PR57)
 - Stop print-syslog.inc.php from shortening hostnames (PR62)
 - Moved some variables from defaults.inc.php to definitions.inc.php (PR66)
 - Fixed title being set correctly (PR73)
 - Added documentation to enable billing module (PR74)

####Improvements
 - Deleting devices now asks for confirmation (PR53)
 - Added ARP discovered device name and IP to eventlog (PR54)
 - Initial updated design release (PR59)
 - Added ifAlias script (PR70)
 - Added console ui (PR72)

###Nov 2013

####Bug fixes
 - Updates to fix arp discovery 

####Improvements
 - Added poller-wrapper (f8debf4)
 - Documentation####Improvements and additions
 - Added auto update feature
 - Visual updates
 - License tidy up started

###Oct 2013

 - Initial release
