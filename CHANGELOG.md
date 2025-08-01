HumHub Changelog
================

1.17.3 (July 17, 2025)
----------------------
- Fix #7484: Use password type on the installation DB config form
- Fix #7486: Catch errors in external file handlers
- Fix #7487: Fix comments list when comment is active from another parent comment
- Enh #7492: Fix access to options on space invite form
- Fix #7503: Don't run migration on updating of disabled module
- Fix #7513: Fix priority of `dynamic.php`
- Enh #7514: Update Redis example in `env.example`
- Fix #7532: Prevent multiple execution of jobs canceled due to max. execution time.
- Enh #7549: Allow logout from Mobile App
- Enh #7546: Improve member space list box
- Fix #7560: Fix SafeBaseUrl to not repeat the `base URL` in the `script URL`
- Fix #7563: Top padding on medium screen size for some themes such as Entreprise theme
- Fix #7570: Fix `CodeMirrorInputWidget` in collapsible fields
- Fix #7573: Update test user passwords
- Enh #7577: Increase Group Name max length to 120chars
- Enh #7576: Do not invite existing space members when selected `all registered members`
- Enh #7579: Mail headers to restrict auto-reply

1.17.2 (April 7, 2025)
----------------------
- Fix #7457: Fix changing of space visibility
- Fix #7464: Fix searching with not full latin words
- Fix #7465: Formatted Arabic numbers displays 0 instead of the number
- Fix #7471: Fix advanced searching by space filter
- Fix #7472: Fix missing fields when creating a new user from admin
- Fix #7477: Refactor Registration Form Options 
- Enh #7455: Add Share Intend feature for the Mobile app
- Fix #7482: Fix the post submit button title after back from draft mode

1.17.1 (March 6, 2025)
----------------------
- Fix #7377: Configured Redis cache key prefix was overwritten by the default value
- Fix #7375: Use default language for email invitation and show language chooser on registration form
- Enh #7383: Improve SelfTest for Base URL 
- Enh #5426: Show language chooser for guest on the sidebar footer
- Fix #7395: Fix profile stream for guests
- Fix #7400: Fixed `Default user profile visibility` field visibility in the user settings
- Fix #7404: Marketplace - Allow symlinked `@app/modules` directory
- Fix: Always allow admins to edit/delete content in the other Profile stream
- Fix #7414: Fix profile field encoding
- Fix #7419: Reset modal window after close
- Fix #7428: Fix picker autofocus
- Enh #7424: New event on get registration groups
- Enh #7437: Add beforeInitCallback `humhub.ui.picker`
- Fix #7441: Hide "Remember me" option on mobile app
- Enh #7408: Update code to manage users from external modules
- Fix #7453: Fix registration form submit

1.17.0 (January 13, 2025)
-------------------------

See also: HumHub 1.17 - [Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_17) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

Info: The minimum PHP version is now `PHP 8.1`!

- Fix #7365: `DeviceDetectorHelper::isMobile()` and `DeviceDetectorHelper::isTablet()` when no user agent
- Fix #7376: `humhub\helpers\ArrayHelper::flatten()` not compatible Yii base ArrayHelper
- Enh #7382: Allow initial collapsed comments bu setting `\humhub\modules\comment\Module::$commentsPreviewMax` to 0

1.17.0-beta.4 (December 24, 2024)
---------------------------------
- Enh #7307: Improve request scheme detection
- Fix #7308: Fix Hungarian symbol error in `Open Sans` font
- Fix #7309: Fix style of the "Notification Settings" button on small screen
- Fix #7312: Auto refresh a page with violated script-src because of obsolete nonce
- Fix #7308: Fix Hungarian symbol error in `Open Sans` font 
- Fix #454: Profile about page missing left and right margin on mobile screen
- Fix #7316: Fix formatter default time zone
- Enh #7317: Space browser: Make the whole space card header and body clickable
- Enh #7329: Add a new "Manage All Content" Group Permission (see [migration guide](https://github.com/humhub/humhub/blob/develop/MIGRATE-DEV.md#version-117-unreleased) for details)
- Enh #7325: Add missing IDs in the modal login forms
- Enh #7333: Improved Yii alias handling and added ENV support
- Enh #7334: New safe method to rename a database column
- Enh #7336: Update GitHub workflow versions
- Enh #7339: Add `DeviceDetectorHelper::isMultiInstanceApp()` method to detect if the app is running in a multi-instance mode
- Enh #7342: Mask .env `DB__PASSWORD` variable in logs
- Enh #7344: Disable editing Base URL when setting is fixed
- Fix #7345: Fix debug mode setting in .env
- Enh #7349: Add body classes about the current device and methods to the `DeviceDetectorHelper` class
- Enh #7353: Enable dot env to read variables based on application type

1.17.0-beta.2 (November 12, 2024)
---------------------------------
- Enh #7280: Allow to add a space as default for new users from "Invite members" modal window
- Fix #7281: SelfTest for DynamicConfig broken when not exist yet
- Fix #7284: Content tag visibility
- Enh #7287: Add `Template` virtual field
- Enh #7291: Disable link in `TopicLabel` when contentContainer is not present
- Enh #7293: Add Twig string extension
- Fix #7287: Fix `Profile::getFormDefinition` to skip virtual fields
- Fix #7295: iOS mobile app detection for iPad devices
- Fix #7299: Fix public content from spaces on the profile in guest access mode
- Fix #7301: Profile header: on small screens, the space at the left and the right of the image must be equal   
- Fix #7298: Don't check email for existing on password recovery (CVE-2024-52043)
- Enh #7038: Optimize notification overview
- Enh #7346: Change cache settings keys to meet dot env naming

1.17.0-beta.1 (October 28, 2024)
--------------------------------
- Enh #7070: Add GitHub action for PHP CS Fixer
- Enh #7073: Add a link to notification settings on top dropdown list
- Fix #7100: Enable all file handlers on RichText editor toolbar
- Enh #7127: Prerequisites - Check that Web and Cli php version and user is the same
- Enh #7128: Prerequisites - check for mixed table collations
- Enh #7131: Introduce new CSS variables: `--hh-fixed-header-height` and `--hh-fixed-footer-height`
- Enh #7129: Link `wall-entry-controls`- color to `--text-color-soft`
- Chg #7136: When opening a modal box, don't autofocus automatically on the first form input
- Enh #7138: Added missing DB relations to UserInvite model
- Enh #7139: Export `confirmUnload` function from `humhub.client.js`
- Enh #7068: Bulk re-send email invites
- Enh #7144: Add `DeviceDetectorHelper` class to detect devices such as the mobile app
- Fix #7149: Fixed dropdown issue on mobile
- Fix #7151: Disable new post's required validation for `message` when post has attached files
- Enh #7106: Enable option for non-member users of a space to create posts
- Enh #7160: Default state set to Deny for `Create Private Spaces` and `Create Public Spaces` Groups permissions
- Enh #7166: When browsing HumHub from the mobile app, add a warning to the dashboard (`IncompleteSetupWarning` widget) if HumHub doesn't support push notifications
- Fix #7174: In lists, when an item text is displayed on multiple lines, the lines below are not lining up with the first one
- Fix #7173: Fix marketplace module label "Professional Edition"
- Fix #7176: Fix of broken tests related to `Create Private Spaces` and `Create Public Spaces` Groups permissions
- Enh #7198: Increase default Upload Max File Size to 64mb
- Fix #7197: Increased version of `PHPOffice/PHPSpreadsheet` to v2.2+
- Enh #7167: Disable DEBUG mode automatically after successful humhub installation. Add `.env` support
- Enh #7202: Increased minimum PHP version to 8.1
- Enh #7208: Improvements in dotenv parsing
- Enh #7213: By default, enabled "Mobile" notification types for those enabled for "Web"
- Fix #7215: Wording: replace British "licence" with American "license"
- Fix #6987: Added LatAm Spanish
- Enh #7214: Replace theme variables with CSS variables
- Enh #7221: Increase language column size for new language codes
- Enh #7226: Added configuration option for default stream sorting on space level
- Enh #7224: Added `user\Module::$invitesTimeToLiveInDays` to automatically clean up User Invites after a specified number of days
- Enh #7231: Removed deprecated `ShowMorePager` widget
- Fix #7230: Update module with new id
- Enh #7234: Remove using of database timezone
- Enh #7233: Mobile view: enlarge images in gallery preview of entries for the wall stream
- Enh #7237: Changed PoweredBy URL
- Enh #7238: Fixed PHP warning related to `.env`
- Enh #7239: Added option `\humhub\modules\installer\Module::$enableAutoSetup` to enable/disable auto setup of humhub installation
- Enh #7240: Fixed maximum file size setting in initialization
- Enh #7244: Changed .env var depth separator from `.` to `__`
- Enh #7251: Commands for module info and test DB connection
- Fix #7248: Upgrade jQuery Highlight plugin
- Fix #7254: Fix Login view HTML element ID from `user-auth-login-modal` to `user-auth-login`
- Fix #7250: Check writable path
- Enh #7255: Improved CSP headers
- Enh #7253: CSV/XLSX export improvements
- Enh #7252: Show "Powered by HumHub" even if no entries in the Footer menu
- Enh #7257: Move "About" into Space Control Menu
- Enh #7262: Disable `Like` on archived content
- Enh #7125: Prerequisites - Check test for pending migrations
- Fix #173 : Remove UISetting "Include Captcha in Registr
- Fix #7066: Allow using `Space::canJoin($userId)` in command line
- Enh #7037: Space creation notification to users allowed to manage spaces
- Enh #7243: Server time zone
- Enh #7188: Helper for detecting a current path by module/controller/action
- Enh #7265: Profile "About" page: don't display the menu if only one entry
- Enh #7269: Remove desktop notifications
- Enh #5423: Display password rules in form field hint
- Enh #7223: Global Topics
- Enh #7274: Restrict user content visibility on Dashboard for guests

1.16.3 (Unreleased)
--------------------------
- Fix #7212: Fix horizontal scroll bar on space stream on small screen
- Fix #7210: Small style fix for top account menu (temp fix for Mac Safari browser)
- Fix #7218: Fix visibility of wall stream content creating form
- Fix #7219: Renamed deprecated meta tag
- Fix #7174: In lists, when an item text is displayed on multiple lines, the lines below are not lining up with the first one
- Fix #7222: Fix rendering of checkbox on MacOS and iOS
- Fix #7225: Fix module JS config initialisation on AJAX request
- Fix #7227: Fix search reindexing after create new content
- Fix #7232: Refresh the `updated_at` timestamp of invitation after resend it
- Fix #7241: Fix file visibility for object with viewable interface
- Enh #7229: Hide invitations with unknown sources
- Fix #7276: Cron jobs cannot "Create public content" (since 1.15.3)
- Fix #7278: Don't remove html tags by JS from search post record because it is done by PHP
- Fix #7296: Fix email validation of invite new users
- Fix #7319: Display correct profile field value in user subtitle
- Fix #7322: Always allow invitation by link from Administration. Implement separate invitation by link from People.
- Enh #7335: Update GitHub workflow versions
- Fix #7351: Fix caching of space permissions in user stream
- Fix #7297: Auto refresh a page with obsolete nonce value

1.16.2 (September 5, 2024)
--------------------------
- Fix #7102: Fix content search with word ending with hyphen
- Fix #7104: Missing `--text-color-default` CSS variable
- Enh #7105: Add an external link icon to the "Install Updates" button to avoid thinking it updates the modules directly
- Fix #7116: Fix rebuilding the search index with Grunt (since 1.16.0)
- Fix #7120: Error after failed migration of content fulltext index
- Fix #7126: Fix member count on a space directory
- Enh #6794: Improve log wrong parsing of OEmbed URL
- Fix #6794: Add `User-Agent` to oEmbed CURL request (fix for Reddit)
- Fix #7146: Fix search request by container guid
- Fix #7141: Fix meta searching twice for the same keyword
- Fix #7150: Remove js statement `with` to avoid error on build assets by grunt uglify
- Fix #7156: Fix duplicated following spaces in the chooser widget
- Enh #7157: Highlight content after open a page from search results
- Fix #7153: Fix content visibility of disabled users
- Fix #324: Focus on active and selected nav page after reload on mobile
- Fix #7170: Fix rendering of new line on email messages
- Fix #7178: Highlight only words with 3 or more characters
- Fix #7180: Fix active form on registration and user edit forms for correct working of widget inputs
- Fix #7181: Fix duplicated label of checkbox profile field
- Fix #7182: Fix initialization of several select2 inputs on the same page
- Fix #7187: Fix search reindexing after content deletion
- Fix #7152: Fix search starting with special characters
- Enh #7148: Improve rendering of meta search content
- Fix #7192: Deny deleting user from single group
- Fix #7200: Fix module description for space and user
- Enh #7204: Make "Invite new people" always possible for user with permission "Manage Users"

1.16.1 (July 1, 2024)
---------------------
- Fix #7084: Fix compatibility for PHP 8.0+
- Fix #7088: Improve handling of legacy configuration for "search" component
- Fix #7089: Fix markdown sub list style
- Fix #7092: Missing closing `div` HTML tag in the registration by link view
- Enh #7094: Allow color boxes in select2 picker

1.16.0 (June 19, 2024)
----------------------
See also: HumHub 1.16 - [Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_16) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

- Fix #7059: Saving of empty password by admin
- Cgh #7074: Text in lists is smaller than in paragraphs
- Fix #7059: Saving of empty password by admin
- Enh #7067: Display more context menu options on search results
- Fix #7059: Saving of empty password by admin
- Fix #7065: Space members manager crashes on HumHub 1.16.0-beta.3
- Enh #7062: Render emojis also in email content
- Enh #7079: Improve `MenuEntry::isActiveState` to support query params check

1.16.0-beta.3 (June 10, 2024)
-----------------------------
- Fix #5629: Legacy configuration self test not showing "OK"
- Fix #6909: Fix the marketplace searching when a module config file has missed fields
- Enh #6920: Enhancing of meta search for advanced search providers
- Enh #6952: Improve container title encoding in header
- Fix #6954: Search out of viewport on mobile
- Enh #6950: Ability to reset some notification settings to all users without resetting "Like" notifications by email
- Fix #6954: Search out of viewport on mobile
- Fix #6962: People filter - Hide follower options if Following is disabled in the User module
- Fix #6961: Fix people dropdown filter without defined keys
- Fix #6967: Use same order for meta searching that is used for content page searching by default
- Enh #6968: Meta search: open external links in new window
- Fix #6970: MultiSelect loads wrong options (since #6768 in 1.16.0-beta.1)
- Enh #6974: Highlight a content searching keyword on show more comments
- Enh #6971: Meta search: Highlight keyword in single content view
- Fix #6977: Index sub comments for searching
- Fix #6978: Fix module enabling from marketplace
- Enh #6984: In forms, change checkbox style to match other input types
- Enh #6990: Unifying positions of button on modals for consistency and better UX
- Enh #6986: When moving a content from a container to another, prevent updating the content dates to keep the stream sort as it was
- Enh #6992: Improve handle database connection errors
- Fix #6552: When a JS file has `module.initOnAjaxLoad = true;`, if the `initOnAjaxUrls` contains multiple params in the URL, the `init` function is not triggered
- Fix #7006: Disable `mustChangePassword` check for impersonated access tokens
- Fix #7004: Fix people filter by group
- Enh #6979: Content Search: use AND operator by default and don't apply mask for phrases
- Fix #7011: Fixed performance issue in `Members::getPrivilegedUserIds`
- Enh #7010: Rich text tables: Vertical align top instead of middle
- Enh #5310: Mobile - Zooming into pictures
- Fix #7017: Fix content search order after restoring from cache
- Fix #7021: Image cropping: prevent vertical images from being displayed higher than the browser window
- Fix #7007: Allow resetting of people filters
- Fix #7023: Fix `Unsupported configuration type: object` Exception when running `php yii` on fresh installation
- Fix #7025: Fix empty password
- Enh #7033: Add search tests
- Enh #7035: Use LESS variables in search.less
- Enh #7041: Marketplace meta search provider
- Enh #6947: Improve meta search record calling for handling from config
- Enh #7053: Search content by ID (mysql driver)
- Enh #7060: Implement new field template radio pills

1.16.0-beta.2 (April 9, 2024)
-----------------------------
- Fix #6928: Disabled users without "ignoredDN" settings
- Fix #5629: Better handling of legacy configuration file options
- Fix #6931: Fix visibility of private spaces in the user notification settings
- Enh #6757: Allow changing visibility of global content
- Fix #5419: Lock search index while reindexing
- Fix #5629: Better handling of legacy configuration file options for disabled non-core modules
- Enh #6976: Migrate to PhpSpreadsheet 2.0

1.16.0-beta.1 (April 5, 2024)
-----------------------------
- Fix #6770: Improve migration error messages
- Enh #6750: Code de-duplication by introducing `PermissionManager::handlePermissionStateChange()`
- Fix #6772: Polymorphic relation lookup (Regression #6587)
- Enh #6745: Harmonise term `enabled/disabled` vs `active/inactive` for modules
- Fix #6754: Regression due to return type (#6550)
- Enh #6550: Improve module migrations
- Fix #6237: Migration errors during module activation are ignored
- Enh #6711: run migrations manually
- Enh #6720: Consolidate `isInstalled()`, `setInstalled()`, and `setDatabaseInstalled`
- Fix #6693: `MigrateController::$migrationPathMap` stored rolling sum of migrations
- Enh #6697: Make state badge customizable
- Fix #6636: Module Manager test
- Enh #6587: Apply UUID validator
- Enh #6530: Small performance improvements
- Fix #6511: Only test compatible modules in `onMarketplaceAfterFilterModules()`
- Enh #6511: Backup folder path is now return from `removeModule()`
- Fix #6511: `canRemoveModule` no longer throws an Exception
- Enh #6511: Allow an empty filter list to filter all registered modules
- Enh #6511: Allow module paths for `enableModules()`
- Enh #6511: Verify module's event definition
- Enh #6511: Make module's module.json keywords accessible and searchable
- Enh #6511: Add Event tracking capabilities to HumHubDbTestCase
- Enh #6511: Add test for ModuleManager
- Fix #6519: Ensure e-mails would always have a sender address set
- Enh #6512: Show error messages when DB connection configuration is invalid
- Enh #5315: Default stream sort by `created_at` instead of `id`
- Fix #6337: Update `created_at` after first publishing of content record
- Fix #6631: Fix visibility of the method `Controller::getAccessRules()`
- Enh #6650: Add assets GZIP compression with Apache
- Fix #6662: Change the start_url of the PWA from home to base URL
- Enh #6667: Allow view file when owner object provides this
- Enh #6671: Remove interface `ReadableInterface`
- Enh #5751: Allow user blocking from profile page
- Enh #6486: Add module "Not available" option in spaces or for users
- Enh #6616: Added `data-has-auth-client` in Registration page allowing to know if returning from the SSO provider
- Enh #6686: Make the container header clickable to return to the container's home
- Enh #6609: Monthly email summary
- Fix #6721: Top menu entries for spaces are not highlighted when clicked
- Fix #6725: Allow theme without second topbar menu
- Enh #6760: Change default browser site icon
- Fix #6752: Allow sending a notification to originator when sending to a single user and suppressSendToOriginator is false
- Enh #131: Online Indicator- People Cards, Members Snippet, My Profile
- Enh #6335: Pending approvals: possibility to send a message
- Fix #6774: When enableMailSummaries is false in the configuration file, prevent accessing the "E-Mail Summaries" page in the account settings
- Fix #6777: Allow access to pending registrations to non-system admins
- Enh #6783: Lowercase user email before save
- Enh #6786: Improve password hashing
- Enh #6788: Allow to disable login/registration form via configuration file
- Enh #6788: Allow new user registration of specified SSO providers via configuration file
- Fix #6790: Fix marketplace searching
- Fix #6811: `SpaceModelMembership::removeMember()` should always return a boolean value (returns void if success)
- Fix #6808: On small screens, in the "Spaces" page, for spaces not having an image, the acronym text is not vertically centered
- Enh #6812: Reduce people filter options depending on what filtered users have
- Fix #6810: Top menu on small screens: the previous page remains active when the new page is in the drop-down submenu
- Fix #6830: Wrong view filename after module enabling
- Enh #6838: Fix LDAP encryption labels and allow ignore also part of DNs
- Enh #6490: Update button style on force password form
- Enh #6847: Use prosemirror file handler flag
- Fix #6839: The getObjectModel() method should work for all ActiveRecord classes
- Fix #6849: In the "Module Administration" page, remove "Show in Marketplace" for modules not in the `@app/modules` directory
- Fix #6863: If a top menu entry opens a modal box, don't mark it as active when clicked
- Enh #6873: Change people header with selected group
- Fix #6875: On Group::addUser(), if the current user is not logged in (console command or user registration), the method returns false even if the user was added to the group
- Enh #6874: Update open-sans font from composer
- Enh #6707: Uninstalling modules should be done in a background job
- Enh #25: Improve contrast of @default button color
- Fix #6889: Issue with modal boxes when positioning an element at the bottom of the screen
- Enh #6892: Implement new method `getCommentUrl` for comment permanent URL
- Fix #6881: Fix layout styles after run migration
- Enh #6904: Content Search: Add Tests regarding `state`
- Enh #2758: Make sure we understand how to configure who receives notifications about new users to approve
- Fix #6908: Fix default mentioning URL
- Enh #6879: Better UX for the maintenance mode administration form
- Enh #6901: Auto load pages on content search
- Fix #6913: Fix API tests
- Fix #6730: Invitation link for existing user
- Enh #6147: New space service `MemberListService`
- Enh #6487: Remove general setting "Server Timezone"
- Enh #6552: Allow module initializing on each loading
- Fix #6768: MultiSelect when empty selection is given

1.15.6 (June 10, 2024)
----------------------
- Fix #7013: Opening more auth clients
- Fix #7024: Automatic mapping of existing AuthClient users failed
- Fix #7030: Fix list style near aligned image
- Fix #7024: Automatic mapping of existing AuthClient users failed
- Fix #7044: Don't cache markdown profile field in session
- Fix #7047: Update visibility of activities according to the parent object
- Fix #7050: Fix container setting for broken records
- Fix #7005: Fix flag of new content notification space

1.15.5 (May 8, 2024)
--------------------
- Enh #6899: Fix a missed module config file
- Fix #6913: Fix API tests
- Fix #6919: Fix saving of user profile country field value and enable a searching by country title
- Fix #6919: Migration to revert user profile country names to Iso 3166 codes
- Fix #6966: Make "Invite new people" always possible for Admins
- Fix #6969: Create unique index for the table `like` - Avoid counter manipulation (Thanks to @viliald)
- Fix #6973: Fix wide dropdown on small screens
- Fix #6869: Display notifications only of published contents

1.15.4 (March 20, 2024)
-----------------------
- Enh #6888: Better support for custom caches
- Fix #6851: Update HumHub Prosemirror (fixes legacy emoji support)
- Fix #6859: Hide scheduled and draft content on other user profile pages
- Fix #6871: Cache is not deleted after deleting a value in the settings
- Fix #6894: Fix obsolete notifications
- Fix #6897: Fix clearing of "Follow" records on space deletion

1.15.3 (February 8, 2024)
-------------------------
- Fix #6713: Keep class option for Pjax Widget
- Enh #6779: Added Twig Sandbox Extension for Statistic Tracking Codes
- Fix #6791: Fix number of filtered modules on Marketplace
- Fix #6744: Make sure to call `humhub\components\Module::update()` on Module updates
- Fix #6796: Files in the RichText doesn't open as new tab
- Fix #6800: Fix missed domain of profile url in email notifications
- Fix #6801: Add missed twemoji images
- Fix: Iso3166Codes class calls
- Fix #6813: Fix for displaying whether I follow a user
- Fix #6126: `Session::$timeout` takes effect before configured `User::$authTimeout`
- Fix #6795: Fix searching of disabled users in Administration
- Fix #6834: Fix notification switcher in wall stream entry context menu
- Fix #6836: Fix check permission of changing content to public from context menu
- Fix #6837: Fix saving of public content

1.15.2 (December 19, 2023)
--------------------------
- Fix #6753: Non-unique key used for permission caching
- Fix #6741: Fix no pretty url of password recovery link
- Enh #6734: Trim Base URL on save
- Fix #6708: Fix displaying of alert when RichText is changed on refresh a page
- Fix #6747: Fix loading of default container permissions from cache
- Fix #6766: Since Humhub 1.15.1, getting content polymorphic relation changes the content object_model to the wrong class

1.15.1 (December 13, 2023)
-------------------------
- Enh #6697: Make state badge customizable
- Fix #6698: Content relations
- Fix #6644: Fix push service
- Fix #6645: File dropdown not visible at the bottom of the page
- Fix #6639: Apply image inline styles in email message
- Fix #6649: Fix birthday format on welcome page
- Fix #6656: Fix people and space filters
- Fix #6652: Fix profile update on welcome page
- Fix #6660: Fix memory usage on integrity check
- Fix #6666: Limit jQuery with version < 3.7.0 to avoid dropdown error
- Fix #6653: URL in email notification removes the sub-folder of the Base URL
- Fix #6674: Fix visibility of draft and scheduled content on dashboard
- Fix #6679: On the space invitation by link page, the language chooser doesn't save the selected language
- Fix #6677: Do not check mobile push module in requirements check on installation
- Fix #6678: Refactor auto start tour for new user
- Fix #6694: Remove the "Offline" tooltip when my own "Online" status is not displayed
- Fix #6700: Reload theme variable `@baseTheme` after flushing cache

1.15.0 (November 6, 2023)
--------------------------------

See also: HumHub 1.15 - [Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_15) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

Warning: HumHub now employs JavaScript nonces for enhanced security (CSP), which may necessitate manual adjustments for inserted scripts, such as statistics codes, to ensure compatibility. See [Migration Notes](https://docs.humhub.org/docs/admin/updating-migration2#115) for details.

- Enh #6619: Add a link to "Module Administration" from Marketplace
- Enh #6620: Marketplace: Add more module checks
- Enh #6621: Avoid PHP error when trying to download a file without guid in the URL params (return 404 exception instead)
- Enh #6623: Add a hint in the "Dropdown space order" settings to inform that a manual sort is always applied first
- Enh #6626: Content state flag "was published"
- Enh #6628: Add self test check: "Mobile App - Push Service"
- Fix #6634: Refresh cache after set a permission
- Fix #6638: Padding for logo image on login page

1.15.0-beta.2 (October 5, 2023)
-------------------------------
- Enh #6594: Add field `file.metadata`
- Enh #6593: Add field `file.sort_order`
- Enh #6592: Add field `file.state`
- Enh #6591: Add field `file.category`
- Enh #6568: improve UUID validation and add `UUIDValidater`
- Enh #6553: Support log assertions
- Fix #6551: Migration's transaction with invalid savepoint
- Fix #6549: Empty profile field type causing an unspecific error
- Fix #6547: Invalid class name validated as valid and improve validation
- Enh #6529: Add boolean return-type to `*safe*` methods in migrations
- Fix #6516: Humhub test case would fail on skipped tests
- Enh #6478: Add pseudo test class to allow population of DB with standard test data
- Enh #6480: Convert assert* and db* methods to static, in line with general usage pattern
- Enh #6505: Introduce Application interface; now also fire the `onInit` event when the web application has initialized
- Fix #6502: Link notification for pending space approval to manage page
- Fix #6472: Initialization of account profile field type "Markdown"
- Fix #6471: Wording "Default Homepage" in Space Default Settings
- Fix #6468: Module Administration - Marketplace Links broken without Pretty URLs
- Enh #6469: Added Info text for Marketplace page
- Fix #112: Reorder Table Rows
- Fix #6476: Fix module disabling in queue
- Enh #6469: Implement conditions for `fixed-settings` in config
- Enh #68: Online Indicator Position
- Fix #6492: Fix module form "Set as default"
- Fix #6457: Regression with membership cache. Also move cache to `Membership::findMembership`.
- Enh #6498: Implement option "disabled" for picker fields
- Enh #6506: Allow event data from module config
- Fix #6510: Fix online status position on people page
- Fix #6526: Fix a disabled button after post a content record with state "Draft" or "Scheduled"
- Fix #6537: Sort profile fields on People directory filters
- Fix #6558: Avoid PHP 8.1+ deprecated null parameter on preg_replace in richtext converters
- Fix #6544: Registration not possible with SSO and email invites if "New users can register" is disabled
- Fix #6572: Posts count in space should be only for published content
- Fix #3755: Fix default oembed styles for twitter posts
- Fix #6582: Enabled `RuntimeCache` during tests
- Fix #6583: Refresh modules available updates counter after updating of modules
- Fix #6585: Exclude database views on self checking

1.15.0-beta.1 (July 31, 2023)
-----------------------------
- Fix #6461: Test server support to serve web module's `/manifest.json`, `/sw.js`, & `/offline.pwa.html`
- Enh #6460: Test server output: print application requests
- Fix #6423: log.fata in frontend logging is redirected to log.fatal, which did not work
- Fix #6220: User Soft Delete doesn't remove third party auth references
- Enh #6270: Add tests for SettingsManager
- Enh #6272: Always return integer from settings, if value can be converted
- Fix #6267: SettingsManager::flushContentContainer() only clears the collection in the current instance, not the underlying cache
- Enh #6271: Add input and type checks, as well as strict types to SettingsManager
- Fix #6266: BaseSettingsManager::deleteAll() does use prefix as wildcard
- Fix #6259: Add json & pdo extensions as requirement; updating composer dependencies and node modules
- Fix #6192: Where Group::getAdminGroupId() would sometimes return int, sometimes string
- Enh #6260: Improve migration class
- Fix #6199: Module manager Add types to properties
- Fix #6189: Module settings survive deactivation in cache
- Enh #6236: Logging: Show log entries from migrations with category migration
- Fix #6216: Spaces icon in admin menu
- Chg #6212: Revise email sender (always use the system name)
- Fix #6229: Bug on saving forms: Zend OPcache API is restricted by "restrict_api"
- Enh #6225: Removed deprecated MarkdownEditor usages
- Enh #6240: Add ability to set showAtDashboard in SpaceMembership::addMember method
- Enh #6164: Invitation by link: when registering within an SSO, the email should only be requested on the service provider
- Enh #6240: Add ability to set showAtDashboard in SpaceMembership::addMember method
- Enh #5668: Allow Admin to sort the Spaces in a custom order
- Enh #29: AutoStart Tour for new Users
- Fix #6243: Do not send notification when ApprovalRequest is not valid
- Enh #6215: Added `LongRunningActiveJob` to avoid timeout for long running queue jobs
- Enh #6253: Remove `DefaultSwipeOnMobile` checkbox
- Enh #10: Added `collapsedPostHeight` to the Post module for set collapsed post default height
- Enh #6277: Bring back Pjax Functionality
- Enh #6285: Change background color for confirmation of oembed content
- Enh #6289: Refactored UserWall and Wall widgets
- Fix #44: Mail Module Indicator Problem
- Enh #6295: Add the possibility to display if users are online
- Fix #6299: Fix ambiguous space sort order column
- Enh #2590: Possibility to add a dropdown button to upload audio, image or video file type
- Enh #6298: Move the "Write a new comment" field style to a generic field that can be used by other modules
- Enh #6310: Module information is localized with `docs/uk/README.md` or `README.uk.md`.
- Enh #6311: Added {cols, rows} to textarea() control.
- Enh #6304: Update button title on creating of not published content
- Enh #6319: Duplicate File Converter Logs
- Fix #5962: Make top menu shrink and grow on resize window
- Enh #6328: Add arrows for gridview sort columns
- Enh #6327: PHP error when calling `Password::setPassword` on unsaved User records
- Enh #2: Store Default Markdown Editor Mode
- Enh #6355: Fix limit results in People: Country Filter
- Enh #6327: PHP error when calling `Password::setPassword` on unsaved User records
- Enh #6356: Added SqlDataProvider support for `ImageColumn` and `DisplayNameColumn`
- Enh #6169: Replace deprecated `yii\base\BaseObject::className()`
- Enh #6361: Use `LongRunningActiveJob` on more active jobs
- Enh #6363: Add an event in the NotificationManager to allow removing some notifications categories in the settings
- Enh #6371: Space Hide Member Option disables Member Joined/Left Activities
- Enh #6375: Performance Improvements
- Enh #6369: Don't pin draft and scheduled contents on dashboard
- Enh #6370: Remove FlatElements CSS
- Enh #6379: Normalize integer columns after load data to ActiveRecord
- Enh #6384: Added Serbian(sr) language
- Enh #6389: Remove deprecated JS function `setModalLoader()`
- Enh #6394: Removed custom DateValidator.php after Yii 2.0.48 release
- Enh #6393: The installer should clear all caches early
- Fix #6391: Fix initialization of account profile field type "Markdown"
- Enh #5713: Disabling modules will be done in a background job
- Enh #6400: Enable nonce in config web header
- Enh #6405: Uploading a file larger than PHP's limits does not tell the user about the file weight issue
- Enh #6407: FileHandlerButtonDropdown - Possibility to have a custom CSS class
- Enh #6130: Add default settings for space creation
- Enh #6079: Migrated Content Tag Logic into `ContentTagService`
- Enh #5718: Use Select2 plugin for all drop-down list fields
- Enh #6132: Widget `AjaxButton` now deprecated. Consider use `data-action` instead
- Enh #6411: Make invite by link from a space work for registered users
- Enh #6409: Redirect to the invited space after registration
- Enh #6386: Fix absolute base URL in console commands
- Fix #79: Fix Headline HelpText Style
- Fix #6418: Fix login from modal window
- Fix #6395: Link notification for pending space approval to manage page
- Fix #6415: Fix caching keys on space directory
- Fix #6424: Fix width of select2 dropdown inputs
- Fix #6425: Fix default dropdown select2 options
- Fix #6428: Translation for custom profile field is served from wrong file
- Fix #6429: Fix Marketplace view
- Fix #6383: Remove permission verifying from archive methods
- Enh #6439: Add collapsible filter state in URL
- Chg #6174: Users allowed to manage settings can access to module configurations
- Enh #6440: Sort user groups by `group.sort_order` and alphabetically
- Enh #6454: Account deletion confirmation
- Enh #6458: Redirect to the latest-visited page after login or registration

1.14.5 (November 6, 2023)
-------------------------
- Fix #6596: Fix duplicate error and hint for RichText editor with defined form
- Fix #6595: Fix mimetype of converted preview svg file to png after uploading
- Fix #6614: Fix undefined error on live event of follow action
- Fix #6615: Improve scrolling to anchor with fixed header
- Fix #6629: Fix visibility of new message counter on space chooser
- Fix #6630: Fix visibility of top sorted stream entries on dashboard from external filters
- Fix #6635: Fix visibility of the method `Controller::getAccessRules()`

1.14.4 (September 20, 2023)
---------------------------
- Fix #6489: Never delete original file on store new version
- Fix #6507: Reload page after accepting of invite in Space header
- Fix #6531: Fix active style for `btn-lg`
- Fix #6534: Cannot change Homepage of space in PHP 8.x
- Fix #6543: Fix errors of inside modal actions
- Fix #6539: Fix overriding of loaded value with default value on HForm
- Fix #6464: Fix access to own user container
- Fix #6349: Fix error on login new user from external service when maintenance is enabled
- Fix #6557: Fix not initialized groups array on the module administration
- Fix #6556: Fix command `theme/switch`
- Fix #6574: Improve a sort order of wall entry creating tab menu and form
- Fix #6577: Wrong usage of user model scenarios
- Fix #6578: Refactor user edit form

1.14.3 (July 27, 2023)
----------------------
- Fix #6345: Fix updating of post on wall stream
- Fix #6351: Error when config `defaultReloadableScripts` is not array
- Fix #6359: Avoid double call of `afterSave` on creating of a published content
- Fix #6373: Use integer format for Content columns "visibility" and "state" right after creating
- Fix #6377: Forgot Password - Display email input error after successful captcha verification.
- Fix #6378: Fix visibility of the link "Uninstall" on Windows server
- Fix #6404: Fix visibility of global content on dashboard for registered users
- Fix #6441: Display topics and content types in filters header on load page with selected filters
- Fix #6433: Avoid duplicate activities on save published content

1.14.2 (May 22, 2023)
----------------------
- Fix #6257: Editing Draft lead to unexpected error
- Fix #6333: Fix installer crash on fresh installs
- Fix #6342: Fix broken file uploading

1.14.1 (May 15, 2023)
---------------------
- Fix #6251: Emulate execution on `readable()` content
- Enh #6252: Implement new method to handle changing of content active record state
- Enh #6248: If admins can view all contents, users allowed to manage spaces or users cannot view all content (they should be able)
- Enh #6255: Updated activities to same state as parent record
- Enh #6248: If admins can view all contents, users allowed to manage spaces or users cannot view all content (they should be able)
- Fix #6264: Fix date format for columns `created_at` and `updated_at`
- Fix #6265: Broken HMTL in Visibility and Hidden Checkbox
- Enh #6242: Submit button hidden when editing a comment having a long "code" line
- Fix #6282: Hard delete content records on integrity check
- Fix #6257: Fix error after publishing of a draft content
- Fix #6258: Send notification to mentioned user only after publishing of a content
- Fix #6273: Fix automatically login user after registration
- Fix #6292: Messages: Notification Indicator Problem
- Fix #6296: Update style variable `background-color-secondary`
- Fix #6228: Administrators allowed to manage users cannot invite by email or by link if disabled in the settings
- Fix #6293: Delete content from DB completely on purge content by cron job
- Fix #6316: Dashboard Activity Sidebar Loading Speed
- Fix #6262: Fix visibility of deleted content

1.14.0 (April 20, 2023)
-----------------------
- Fix #6196: Use class names for default logging targets in default common config
- Fix #6202: Invite by link is not possible for a user already invited by email
- Fix #5718: Fix profile field "Country" to use js plugin Select2
- Enh #6214: Improved SoftDelete implementation
- Fix #6221: Improved SaaS handling in installer
- Fix #6232: Fix Error DateValidator::parseDateValuePHP in php8.2
- Fix #6246: Can change email in `AccountController`

1.14.0-beta.2 (March 28, 2023)
------------------------------
- Enh #6173: Theme variables background-color-highlight and background-color-highlight-soft
- Fix #6099: Empty buttons in GlobalConfirmModal footer
- Fix #6100: Broken area reference in some modal boxes
- Enh #6171: Make email in user administration and user approval clickable
- Enh #6184: Use same font for RichText editor as it looks on view mode
- Enh #6181: Replace png "search" icon with font-awesome icon
- Fix #5537: Space Starting Page gets lost when changing URL
- Enh #5681: People: Add Group Description
- Enh #6197: Updated translations. User module. Ukrainian
- Enh #6187: Deny custom input for Space Picker field

1.14.0-beta.1 (March 10, 2023)
------------------------------
- Enh #4803: Added more panel styles (panel-info and panel-primary)
- Enh #5972: Removed old vendor CSS prefixes (e.g. -moz or -webkit)
- Enh #6006: Fix activity settings test
- Fix #6018: Disable profile fields textarea and checkbox list when they are not editable
- Ehn #6017: Hide Password Tab in administration for LDAP users
- Enh #6031: On users list grid, show Auth mode badge only for sys admins
- Enh #6033: Moved more logic into AbstractQueryContentContainer
- Enh #6035: Added Estonian language
- Fix #5956: Display all newer comments after current comment
- Enh #6061: Administration: Add a confirmation on profile field delete button
- Enh #5699: Allow users to invite by link
- Enh #6081: Added corresponding CSS variables for LESS color variables
- Fix #6022: Fix Changelog Link with new Marketplace URL
- Enh #5973: Stylesheet Prefix Cleanup and removed temporary style
- Enh #6077: Always display content tabs
- Enh #5263: Allow members of groups other than system admin to view all content (groups that can manage users for profile content and groups that can - manage spaces for space content)
- Enh #6102: Also allow Messages module to inject new message count into page title
- Enh #6109: Added enabled Pretty URL as self test
- Fix #6113: Ensure displayNameSub doesn't return NULL values
- Enh #5904: Make Dynamic Post Font Size Optional
- Enh #6109: Added enabled Pretty URL as self test
- Enh #6119: Added UserInfoWidget for User Notification Settings
- Enh #6116: Scheduled content publishing
- Enh #6135: Added new ContentState and Content events (e.g. SoftDelete)
- Enh #5625: Update jQuery UI to version 1.13
- Enh #6144: Added ability to change/disable Forgot your password? link
- Fix #4988: Unable to archive space on Form Validation errors
- Enh #6123: Added check for proc_open function in Requirement Checker
- Enh #6149: Added AuthClientUserService and AuthClientService instead of AuthClientHelpers
- Enh #4712: When changing space Visibility to Private, the all content visibility will be changed to private too

1.13.3 (Unreleased)
--------------------
- Fix #6195: Fix `ModuleManager` disabling logging when no modules set

1.13.2 (March 27, 2023)
-----------------------
- Fix #5965: Suppress log warning 'Invalid session auth key attempted for user'
- Fix #6084: Automatic LDAP user registration broken when not all req. attributes provided
- Fix #6104: Fix update user with not existing group
- Fix #6103: Fix null passing to parse_str()
- Fix #6108: Fix log time in the `date()` function
- Fix #6122: Fix deleting a content with empty reason
- Fix #6128: Reset backuped content after submit form
- Fix #6141: Hide invisible users on People page even for admins
- Fix #6142: Fix saving empty values in admin settings
- Fix #6145: Fix duplicate people cards on sort
- Fix #6152: Avoid duplicate container(Space/User) tags on save
- Fix #6182: Fix Date and Datetime profile field type with null values on PHP 8.1+

1.13.1 (January 25, 2023)
-------------------------
- Fix #5985: Space user search in picker
- Fix #5993: Broken images on installations with multiple URLs
- Fix #5996: Fix param type in strpos() (PHP 8.1)
- Fix #5997: Possible NULL param value in Birthday field (PHP 8.1)
- Enh #6001: Added new `ContentActiveFixture` and migrated `PostFixture` to it
- Fix #6007: Fix number of space members
- Fix #6012: View own invisible profile
- Fix #6027: Fix private user visibility by guest
- Fix #6030: Use all searchable profile fields in UserPicker searching
- Fix #6026: Fix visibility members counter for guests
- Fix #6041: Fix search of obsolete cached objects
- Fix #6043: Fix permission to lock/unlock comment for admin
- Fix #6051: Fix visibility of "NEW UPDATES AVAILABLE!" for space creator
- Fix #6055: Fix click event of notification filter
- Fix #6054: Fix pagination after filter notifications

1.13.0 (December 21, 2022)
--------------------------
See also: HumHub 1.12 - [Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_13) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

- Fix #5954: Clear margin bottom of fieldset control label
- Fix #5958: Fixed members list in Space overview when Space members are hidden
- Fix #5980: ModuleManager - Module Info is not cached properly
- Fix #5982: Use modules method getContentContainerName in ContentContainer module overview

1.13.0-beta.2 (29 November, 2022)
---------------------------------
- Enh #5951: Added default spacing between icon and text inside buttons
- Fix #5950: Fixed failing updater when user:auth_key is not applied yet
- Fix #5953: Display issue left border from divider of dropdown menu

1.13.0-beta.1 (28 November, 2022)
---------------------------------
- Enh #5821: Remove "regular" style of checkbox and radio
- Enh #5827: Wall menu tabs for create content forms
- Enh #5808: Add a menu to remove all members of a space
- Enh #5841: Possibility to show Members/Followers as list from Space about page
- Enh #5850: Display all levels by default on info logging page
- Enh #5864: Use Base URL from general settings for all generated absolute URLs
- Enh #5868 #3506: Add Open Graph support to have preview of the pages on other websites (Facebook, Twitter, etc.)
- Enh #5872: Invalidate active sessions after password changing
- Enh #5820: Selftest for base URL
- Enh #5891: Improve select2 width on people filters
- Enh #5894: Remove EE from Licence Manager
- Fix #5903: ContentContainerModule::getEnabledContentContainers() returns an empty array
- Enh #5908: New filter ActiveQueryUser->available()
- Enh #5785: Adding option for custom .well-known routes
- Enh #5100: Added SelfTest for HumHub API connectivity
- Enh #5811: Don't require current password if not exists on force change password
- Enh #5913: Possibility to configure the "Follow" activity in the e-mail summaries
- Enh #5923: Moved Tour configuration from Config Params to Module class
- Enh #5924: Auto add secure flag for cookie on detected SSL
- Fix #5926: Renamed default profile field Url to Website URL
- Enh #5686: Add the logo image to the registration page
- Fix #5856: Fixed Mail Settings Help Text SMTPS Port to 465
- Enh #5932: Added advanced space settings Hide About Page, Hide Activity Sidebar Widget, Hide Follower and Hide Members
- Enh #5931: Show Spaces pages always when in Guest Mode
- Enh #5929: Add property createMode for wall stream entry widget

1.12.3 (December 12, 2022)
--------------------------
- Fix #5928: Invalid Mailer DSN breaks whole application
- Fix #5960: Fix cropping of space banner
- Fix #5967: Fix creating of user from administration with enabled notification for default group
- Fix #5966: Fix invalid message pattern without initialized source language

1.12.2 (November 11, 2022)
--------------------------
- Fix #5851: Admin User Settings cannot saved
- Fix #5856: Fix SMTPS Config Migration
- Fix #5854: Don't validate user language on approve
- Fix #5875: LDAP user creation broken without email address
- Fix #5877: Fix wrong empty profile stream message
- Fix #5874: Fix adding licence key after removing it from marketplace
- Enh #5891: Improve select2 width on people filters
- Enh #5906: Allow Space Invites with empty originator
- Fix #5909: Fix optional parameter on ldap user searching

1.12.1 (August 15, 2022)
------------------------
- Fix #5822: Fix content width in mobile view
- Fix #5825: Fix format date to mysql on date stream filter
- Fix #5832: Exception in file open dialog when last update user no longer exists
- Fix #5814: Fix numerated lists in mail summary content
- Fix #5830: Fix cron job of search index rebuilding
- Fix #5838: Fix deprecated null value for `file_exists()` on PHP 8.1
- Enh #5846: Improved PHP minimum version checks
- Fix #5845: Fix unknown `streamQuery` on load `Filter`

1.12.0 (July 27, 2022)
----------------------

See also: HumHub 1.12 - [Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_12) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

- Enh #5788: Limit picker results for country filter on "People" page
- Fix #5779: Fix user settings updating on disabled visibility "Guest"
- Enh #5809: Improve checkbox and radio styles on load page
- Fix #5807: SMTP Mail component not loading with empty `Port` config value

1.12.0-beta.1 (June 27, 2022)
-----------------------------
- Enh #5655: Possibility to archive and lock comments on global contents
- Enh #3593: Allow SSO provider to register and auto create username on registration
- Enh #5695: Truncate long profile texts in People cards
- Enh #5499: Add new Date Range Stream Filter option
- Enh #5602: Added API to inject additional validation rules by modules on demand
- Enh #5741: Possibility to Like global contents
- Enh #5560: Possibility to create custom profile field types via Events
- Enh #5739: Added Event in `MentioningController` raised after searching for space members on mentioning request
- Enh #5752: Improved Display Name Subtitle Usage and Administration
- Enh #5757: Make sure `setupApproved` is always called when status changes
- Enh #5598: Added `cy` Welsh language
- Fix #5338: Content topic/visibility changes are re-indexed in search index
- Enh #5535: Invisible users
- Enh #5747: Switch Mailer Library to `Symfony Mailer`
- Fix #5766: Fix email markdown format
- Enh #5747: Switch Mailer Library to `Symfony Mailer`
- Enh #5769: Added more right margin on wall entries
- Enh #5767: Display placeholder for date filter
- Enh #5747: Switch Mailer Library to `Symfony Mailer`
- Fix #5765: Fix rendering content form on external modules

1.11.5 (Unreleased)
---------------------
- Fix #5806: Alignments for People filters with Select2 mode
- Fix #5813: Fix deprecated null value for hour param in `mktime()`

1.11.4 (July 6, 2022)
---------------------
This release also fixes a [security](https://github.com/humhub/humhub/security/advisories/GHSA-p7h3-73v7-959c) issue. HumHub was vulnerable to a stored Cross-Site Scripting (XSS) vulnerability. For exploitation, the user would need a permission to administer Spaces. An update is STRONGLY recommended.

- Fix #5776: Hide beta modules on disabled filter
- Fix #5799: Incorrect selection when multiple custom filters are in place
- Fix #5780: Don't hide icon "remove item" on picker
- Fix #5800: Hide data of disabled users on picker filters on "People" page
- Fix #5791: Fix XSS in membership confirmation

1.11.3 (June 27, 2022)
----------------------
- Fix: #5736: Fix status message on user approval
- Fix #5734: Fix error message when uninstall module and module folder is not writable
- Fix #5740: Fix logout action on force change password
- Fix #5735: OEmbed migration might fail with more complex Endpoint URLs
- Fix #5760: Fix context menu position on the right window side
- Fix #5759: Fix tests on enable space module
- Fix #5773: Fix PHP 8 incompatibility with conversion false to array
- Fix #5775: Missing encoding of profile labels in profile field administration

1.11.2 (May 30, 2022)
---------------------
- Fix: #5652: Fix undefined UrlOembed provider pattern
- Fix #5660: Individual modules marked with "Official" label in Marketplace
- Fix #5657: Fix links of user counters in container headers
- Fix #5676: Use 404 page for deleted content request
- Fix #5679: Fix message on decline multiple users
- Enh #5690: Use theme colors in marketplace modules
- Fix #5689: Check value on color picker
- Fix #5691: Fix attach file to profile markdown field
- Fix #5693: Scroll to comment on single view
- Fix #5709: Fix input size for placeholder length in picker field
- Fix #5704: Don't send notification for non-member of private space
- Fix #5716: Fix saving of OEmbed provider endpoint URL
- Fix #5706: Fix confirmation window for buttons
- Fix #5724: Deny custom input for UserPicker field
- Fix #5659: Improve module loading error handling

1.11.1 (April 22, 2022)
-----------------------

See also: HumHub 1.11 - [Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_11) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

Warning: The minimum PHP version is now `PHP 7.4`!

- Fix: #5654: Added `laminas/laminas-zendframework-bridge` to legacy support `Zend\Http` usage in 3rd party modules
- Enh: Updated translations

1.11.0 (April 20, 2022)
-----------------------

See also: HumHub 1.11 - [Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_11) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

Warning: The minimum PHP version is now `PHP 7.4`!

- Fix #5637: Allow update setting "include beta updates" on modules page
- Fix #5648: Introduce new config value for min. required PHP version

1.11.0-beta.3 (April 13, 2022)
------------------------------

Warning: The minimum PHP version is now `PHP 7.4`!

- Fix #5603: Syntax error in database view installer
- Fix #5605: Fix warning on render ajax content on register file after View::endPage()
- Fix #5608: Remove duplicated field "Hostname" on install
- Fix #5612: Fix RichText post process event pass data
- Enh #5610: Show menu item "Add Licence Key" for purchased modules
- Enh #5599: Introduce a variables in the Space model to call ProfileImage and ProfileBannerImage classes
- Enh #5621: Optimize footer views
- Fix #5616: Don't display oEmbed confirmation in text field
- Fix #5631: Fix enabling module on functional tests
- Fix #5633: Fix tests NonceCest
- Fix #5635: Fix cached comments

1.11.0-beta.2 (March 18, 2022)
------------------------------

Warning: The minimum PHP version is now `PHP 7.4`!

- Fix #5434: Hide disabled next/prev buttons on guide first/last steps
- Fix #5456: `canImpersonate` only possible for SystemAdmins
- Enh #5462: Added Single Page Post View
- Enh #5476: Rework modules administration section
- Enh #5472: New interface `TabbedFormModel` for activate first tab with error input
- Enh #5224: Add reply-to email in the settings
- Enh #5471: On the pending approval page, add grouped actions and custom columns
- Enh #5490: Display confirmation message before display embedded content
- Enh #5258: Display who invited the user on the Approval page
- Enh #5475: Option for forbidden usernames
- Enh #4890: Allow to define actions in a controller which should not be intercepted by other actions
- Enh #5503: Allow profile fields link prefixes like "tel://"
- Enh #5510: oEmbed support for other social networks, redesign of oEmbed settings pages
- Fix #5534: Statistic input loading problem
- Enh #5523: Option to include E-Mail address to search
- Enh #5352: Remove "NewMembers" widget from Core
- Fix #5478: Avoid permalinks on comments related to a global content (not in a container) to crash.
- Enh #5538: People - Show Text Profile Field Filters as DropDown with AutoComplete
- Fix #5547: Remove Google Fonts from E-mails
- Enh #5536: Optional notification w/ reason when admin deletes content/comment
- Fix #5549: Topic icon is missing in TopicPicker search
- Fix #5556: Formatted output for date fields in "About me" profile area.
- Fix #5553: Cannot have two or more users without email when emailRequired is disabled.
- Fix #5506: Modal: Close Icon optimization
- Fix #5564: Close modal button doesn't work after form validation
- Fix #5533: Users can't live in UTC
- Fix #5460: Untranslatable string New Updates in Stream
- Fix #5573: Allow replying for sub comments
- Fix #5518: Number of activities reported in the mail summary is always limited to 20
- Enh #5358: Remove deprecated "Directory" module
- Fix #5524: Mentioning Permission
- Fix #5529: Tooltip: improving readability
- Enh #5298: Added Followers to Space About Page
- Enh #4558: Deprecate CompatModuleManager
- Enh #5323: Remove deprecated "Setting" classes
- Enh #5381: Optimize module states query
- Enh #4823: Removed CHTML and CActiveForm classes as well as usages (plus refactoring)
- Fix #5449: File - Update info after `setStoredFileContent` and `setStoredFile`
- Enh #5127: LDAP: Reset mapping for single user only
- Enh #5522: Add content id in the file table
- Fix #5581: Fix long words in comment form
- Fix #5578: Improved `rememberMe` parameter handling for thirdparty auth provider
- Fix #5304: In a button, data-action-cancel-text doesn't work
- Fix #5340: Mobile navigation: width detection problem
- Enh #5432: Possibility to add buttons in the People page with a module
- Fix #5585: Don't force password change on user simulating
- Fix #5591: Fix people/space cards banner
- Enh #5575: Add content topics to search

1.10.4 (April 19, 2022)
-----------------------

This release also fixes a [critical security](https://github.com/humhub/humhub/security/advisories/GHSA-2h35-f226-3f57) issue. Users who were forced to change their password by an administrator could perform unauthorized actions and retrieve other users' data. An update is STRONGLY recommended.

- Fix #5480: `el` language file in Admin section broken
- Fix #5479: Fix ContentContainerPermissionAccess without provided container
- Fix #5513: Fix PermaLink controller error for content without container
- Fix #5517: Don't send "Follows" notification on request friendship
- Fix #5563: Limit backup duration of RichText editor for 2 hours
- Enh #5601: Backup RichText in sessionStorage
- Fix #5638: Removed return values from `codeCallback`
- Fix #5634: Fix tests NonceCest
- Fix #5644: Fix console command space/assign-all-members

1.10.3 (December 20, 2021)
--------------------------

See also: [HumHub 1.10 - Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_10) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md). This release also includes a [security fix](https://github.com/humhub/humhub/security/advisories/GHSA-f5hc-5wfr-7v74). It could have been possible for registered users to become unauthorized members of private Spaces. Thanks to [Huntr](https://huntr.dev/bounties/943dad83-f0ed-4c74-ba81-7dfce7ca0ef2/) and @brenu.

- Fix #5465: Fix empty RichText
- Fix #5466: Default `.htaccess.dist` broken
- Fix #5469: Mixed up title for Space membership button
- Fix #5464: Fix comment highlighting on permalink
- Fix #5473: Insufficient member invite check on Space creation

1.10.2 (December 7, 2021)
-------------------------

See also: [HumHub 1.10 - Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_10) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

- Fix #5450: Fix confirmation before close a form with unsaved changes on modal window
- Fix #5453: Fix migration of default group
- Enh #5461: Added Event after a new file content (new version) is stored
- Enh #5457: Use permalink comment in notifications

1.10.1 (November 26, 2021)
--------------------------

See also: [HumHub 1.10 - Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_10) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

- Fix #5445: Checkbox view style unaligned
- Fix #5447: Comments disappeard
- Enh: Updated translations

1.10.0 (November 25, 2021)
---------------------------------

See also: [HumHub 1.10 - Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_10) and [Changelog](https://github.com/humhub/humhub/blob/master/CHANGELOG.md)

- Enh #5437: Tests with MySQL Galera compatibility
- Fix #5427: Fix deep comment link with enabled caching
- Enh #5435: Allow non modal links in header counter
- Enh #5436: Better usage of UserPicker in Form Definition
- Fix #5441: No deletion of file variants in CLI tools
- Fix #5443: Fix misplaced checkboxes on installer forms

1.10.0-beta.3 (November 12, 2021)
---------------------------------
- Enh #5437: Tests with MySQL Galera compatibility
- Fix #5427: Fix deep comment link with enabled caching
- Enh #5435: Allow non modal links in header counter
- Enh #5436: Better usage of UserPicker in Form Definition
- Fix #5441: No deletion of file variants in CLI tools

1.10.0-beta.2 (November 12, 2021)
---------------------------------
- Enh #5403: Confirmation before close a not saved modal form
- Fix #5401: Fix profile field value result type
- Fix #5402: Fix mentioning search in comment content
- Enh #5418: Allow to detach file from simple ActiveRecord

1.10.0-beta.1 (October 27, 2021)
--------------------------------
- Enh #4399: Direct deep links to comments and highlighting
- Enh #4242: More failsafe module loading when reading module config
- Enh #5197: Default `.htaccess` - Remove `Options +FollowSymLinks`
- Enh #4495: Allow locking comments per content
- Enh #3688: Use `Image` widget in user list
- Enh #5194: Confirm leave page for Post & Comment forms
- Enh #5188: People/Spaces: Endless Scrolling
- Enh #5216: Separate View document button
- Enh #5229: Use `RichTextField` for user approval messages
- Enh #100: Allow additional toggle for elements with context menu
- Enh #5170: `UserPicker`: Allow zero as min input size
- Enh #4133: Backup a content of `RichTextEditor`
- Enh #100: Extend upload buttons to use a paste zone
- Enh #5256: Limit uploading profile images (Thanks to @tuhin1729 for discovering the issue.)
- Enh #5257: Delete old unread notifications of inactive users
- Fix #5143: Unlimited page size for profile fields
- Enh #5269: Allow adding new item on ui selector
- Enh #5005: Possibility to invite a registered user to a space by email
- Enh #3546: Sign in back from impersonate mode
- Fix #5282: On account creation, registration form has HTML tag set with English language
- Enh #5280: Allow to set the number of contents from which `Show {i} more.` appears in the stream
- Enh #5303: Unassigned files are only accessibly for creator
- Enh #5293: Added File History API for versioning
- Enh #4399: Changed default `@warning` color to `#FC4A64`
- Enh #5302: Improve checkbox widget ContentVisibilitySelect
- Enh #5151: ContentContainer scoped URL Rules
- Enh #5094: Reflect and reload Stream filters by URL
- Enh $4879: Refactoring of `Followable` behavior
- Enh $4879: Added supported of "protected" module groups
- Enh #5330: Added option to hide "Spaces" top menu item
- Enh #5080: Show available module updates directly in admin menu
- Fix #5331: Fix js error on pjax open "Directory" page
- Enh #5333: Module's events handlers registration: check if method exists
- Enh #5300: Blocking users for space
- Enh #5347: Caching added for group permissions (reduced db queries)
- Enh #5349: Archived Spaces on Spaces directory
- Enh #4945: Collapsible-fields now accessible by tab and enable/closable by keypress, check-boxes now focusable
- Enh #5354: Space - pending invites and approvals: add the image of the users
- Enh #5361: Optimize People directory details query
- Enh #5357: SpaceChooser - lazy load added, widget refactoring.
- Fix #5360: Mentioning search fails apostrophe in a user's displayName
- Fix #5359: Removed encoding of user's name in UserPicker
- Enh #5363: Optimize duplicated SQL queries on profile edit
- Enh #5362: Optimize getting of ContentContainer tags
- Fix #5386: Fixed empty stream in archived space

1.9.3 (Unreleased)
------------------
- Fix #5372: Text shortening in Japanese broken - Fix truncating of multi-byte strings
- Fix #5398: Fix checking of foreign table index

1.9.2 (October 15, 2021)
------------------------
- Fix #5265: Fix logging filter "Error" when not entries
- Fix #5285: Layout too wide for container pages without sidebar
- Fix #5307: Fix reset of the space homepage settings
- Fix #5301: Change people default sorting in administration broken
- Fix #5313: ContentContainer Tags were not cleared when all tags are deleted
- Fix #5316: Fix filter "I'm involved" on dashboard
- Fix #5324: Theme Loader broken when module is provided via string
- Fix #5327: Fix update container tags by not original model
- Fix #5342: Fix mime type detection for extensions: dotx, xltx, potx

1.9.1 (August 30, 2021)
-----------------------

See also: [HumHub 1.9 - Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_9)

- Fix #5172: Missing translations for "New Member" and "New Spaces" directory widgets
- Fix #5195: Fix export users with tags data
- Fix #5200: Auto creating following for friends
- Fix #5187: Fix birthday with hidden year in a language-specific format
- Enh #5189: Reduce minimum character limit for space and user tags to 2 chars
- Enh #5189: Hide tags on space chooser if no keyword inside tags
- Fix #5215: Fix links to old directory
- Fix #5096: Render links in email notifications
- Fix #5095: Fix space between URLs and text in notification message
- Fix #5238: Typo in Offline Page Text
- Fix #5204: Migration of container tags
- Fix #5238: Typo in Offline Page Text
- Fix #5247: Fix translate with not defined language
- Fix #5252: Removed "strong&gt;" from the Dutch translations
- Enh #5259: Protection of the logout action by POST method. (Thanks to @avjesadiya13 and @VishnuChebolu for disclosing the problem.)
- Fix #5262: Fix visibility of email requiring on backoffice add user form

1.9.0 (July 22, 2021)
---------------------

See also: [HumHub 1.9 - Release Notes](https://docs.humhub.org/docs/about/releasenotes/release_notes_1_9)

Note: HumHub version 1.9+ requires PHP 7.3 or higher!

- Fix #5174: Tour module crashes with enabled tags field
- Fix #5176: Closing the action confirmation modal window on top close icon
- Fix #5177: Move directory widgets
- Enh #5049: Required profile field should not be required in administration (Fix for checkbox field type)
- Fix #5009: Fix video thumbnail on Safari browser
- Fix #5182: Password field should not be required if user has no password

1.9.0-beta.2 (July 14, 2021)
----------------------------

Note: HumHub version 1.9+ requires PHP 7.3 or higher!

- Fix #5128: Prerequisites: Increase PHP Min version to 7.3
- Fix #5135: Remove checking for PCNTL extension (revert #5065 and #5071)
- Fix #5136: Fix get value of user profile fields with types "Checkbox List" and "Checkbox"
- Fix #5137: Fix convert to short integer on PHP 8
- Enh #5144: Show sort order in profile fields settings
- Fix #5149: Use a link mode for space button "Join" from space header
- Fix #4830: Fix Prerequisites / Self Test translations
- Fix #4459: Make UserFollow activity public
- Enh #3824: Run acceptance tests with pretty URLs
- Enh #5169: Enable more than 50 groups to a user

1.9.0-beta.1 (June 15, 2021)
----------------------------

Note: HumHub version 1.9+ requires PHP 7.3 or higher!

- Fix #5071: Add CLI hint to PCTL Requirements Warning

1.9.0-beta.1 (June 15, 2021)
----------------------------

Note: HumHub version 1.9+ requires PHP 7.3 or higher!

- Enh #3733: Forbid to open AJAX actions as separate page
- Enh #677: Allow to create new database and set database port on installation wizard
- Fix #4877: Check for writable uploads/profile_image directory
- Enh #4868: Reset email summaries / notifications settings for all users
- Enh #4884: New Space module setting to allow all users to add users without invite
- Enh #4902: Added CodeMirror and created form field widget
- Enh #4964: New CLI command to delete users
- Enh #4871: Configurable default timezone for guests
- Enh #5019: Alternative `DashboardMemberStreamFilter` based on Live module `LegitmationIDs`
- Fix #4626: Visibility of content in profile stream of archived spaces
- Chg #5016: Allow impersonate for `ManageUsers` permission
- Enh #5043: Improved Space membership lookup caching
- Enh #4935: Render images in email messages
- Enh #5037: `RichTextToShortTextConverter` renders images as `[Image]`
- Enh #5042: Improved Space/User PrettyURL performance
- Enh #4958: Add possibility to register purchased modules via CLI
- Enh #4894: Implemented `.label-light` label variant
- Enh #5012: Space: Allow change space owner also for users `ManageSpaces` with permission
- Enh #5045: Removed deprecated `Yii::$app->formatterApp` component
- Enh #5026: Tests for tokenized image urls in email message
- Enh #5049: Required profile field should not be required in administration
- Enh #5065: Add checking for php `PCNTL` extension
- Enh #5073: Enhance Rest API tests
- Fix #5078: Fix enabling of REST module on run API tests
- Enh #4776: Added `acknowledge` option to all relevant forms
- Enh #4757: Updated to `PHPUnit 8.5`
- Enh #4790: Added more logging on authentication errors
- Fix #5054: Force `InnoDB` Table Engine on migration and added engine configuration option
- Enh #4862: Tag picker for Space and User containers
- Enh #4927: Hide post input field on single entry stream
- Enh #5062: Show user ID on admin user edit page
- Enh #4848: Include space tags in the space’s “About” page
- Enh #5061: Preserve linebreaks and added "ReadMore" option in Logging
- Enh #4982: Skip DN List to avoid duplicated ldap error logs
- Fix #5088: Set max length option to space description input
- Enh #5089: Allow to follow users independently of friendship
- Enh #34: Removed membership icon from my Spaces chooser
- Enh #117: Show/Hide the “Following” buttons depending on updated friendship/membership state after AJAX action
- Enh #5102: Use short number format for Space members count on Space Directory
- Fix #5101: Fix to allow admin editing of not required profile fields
- Enh #123: New sorting option "Default" for people directory page
- Fix #122: Fix button "Load more" initialization on Pjax loading
- Enh #5114: Added `EVENT_BEFORE_CHECKING_USER_STATUS` in `AuthController.php` to give the possibility to add an event before checking the user status
- Fix #5122: `RichText::output` produces `p` HTML element instead of `div`

1.8.3 (July 14, 2021)
----------------------
- Fix #29: Fix login form view on browser back button after footer link
- Fix #5066: Fix pin and archive global content without container
- Fix #5107: Fix captcha client validation after request new code
- Fix #22: Fix misplaced OEmbed provider buttons on general settings form
- Fix #5130: Don't require type for first param of the function ProsemirrorRichText::replaceLinkExtension()
- Fix #5155: Open basedir restriction error in with PHP 7.4.21/8.0.8

1.8.2 (April 26, 2021)
----------------------
- Fix #4959: Horizontal scrollbar for images
- Fix #4898: No streamExcludes option when loading single stream entry
- Enh #4960: Added “codeception/module-rest” for testing of REST API modules
- Enh #4976: Added REST API Codeception tester
- Enh #4967: Module update broken with expired licence key
- Enh #4972: Fix enabling to send notification on remove user from group
- Fix #4985: Fix Activity Mail QueryParams on console mode
- Enh #23: Allow to read image URLs with token param
- Fix #4989: Translate profile field title in admin list
- Fix #5002: Fix loading of fixture spaces on tests
- Fix #5018: Activity stream problems with many user accounts
- Fix #5013: XSendFile broken when no SERVER_NAME header provided
- Fix #5004: Preview text maxLength issue
- Fix #5017: File CLI Command fails due to manually deleted files
- Fix #5020: Space visibility options shown to users without permission
- Enh #5024: Disable text wrapping in stream richtext
- Fix #5022: Fix assign default group on user registration
- Fix #5015: Fix visibility of admin menu entries which are initialized with deprecated method
- Fix #5039: RichText converter for some string patterns in HTML format

1.8.1 (March 12, 2021)
----------------------

- Fix #4931: Fix highlight parent navigations for sub section "Profile Permissions" (and LDAP)
- Fix #4934: Show error instead of warning when using different MySQL Table Engines
- Fix #4936: Fix emoji in sample content
- Fix #4940: Typo in German translation "Benachrichtigungen"
- Fix #4942: MemberOf Display in LDAP CLI Show User Details
- Fix #4465: LDAP PHP 8 incompatibility (multiPageSearch)
- Enh #4569: Config to overwrite module path
- Fix #4946: Fix migration of the default permissions
- Fix #4955: Fix convert emoji with sign "+"
- Fix #4956: Fix file hash column length

1.8.0 (March 1, 2021)
---------------------

- Fix #4893: Richtext extension events are ignored when using deprecated maxLength option
- Fix #4896: Error thrown if live poll broadcast focus event is triggered
- Fix #4907: Positions of Comment / Like links under posts
- Fix #4911: Auto logout user on maintenance mode
- Fix #4912: Restrict guest access on maintenance mode
- Fix #4918: Comment richtext gets focused when closing comment section
- Fix #4917: Hide user groups in directory without option "Show At Directory"

1.8.0-beta.2 (February 18, 2021)
--------------------------------

- Fix #4853: Removed obsolete Group::getSpace() relation
- Fix #4828: Display default permissions of all modules even if they are deactivated by default
- Fix #4841: Fix misplaced notification filters
- Fix #4842: Prerequisites Test - Improved database version detection for MariaDB
- Fix #4850: New AuthClient method onSuccessLogin() not available on standard OAuths
- Fix #4856: Allow to invite users to space with pending membership application
- Fix #4869: Fix cached comment content in email notification
- Fix #4857: Fix wrong content id on building cache key
- Fix #4838: ProsemirrorRichText::replaceLinkExtension() not compatible with HumHub < 1.8
- Fix #4847: RichText::postProcess(null) throws error
- Fix #4886: Improved styling of aligned richtext images
- Fix #4891: Typo 'charachters' in chooser message

1.8.0-beta.1 (February 4, 2021)
-------------------------------

- Enh #3996: Force password change on first log in for users created by admin
- Enh #3996: Allow admin to change option "Must change password" for existing users
- Enh #3414: Allow to change user passwords by admin
- Enh #4543: Order members by newest in `about` page
- Enh #4347: Add `hideMembersSidebar` to make members sidebar optional in space stream page
- Enh #4585: Group notifications must be enabled explicitly
- Fix #4646: Clean up duplicated array keys
- Enh #242: Allow multiple default spaces for groups
- Enh #4670: Editable default permissions for Content Containers(Space and User)
- Enh #48: Improve "Admin Can View All" Feature
- Fix #4692: Fix visibility of the button "Add new space"
- Enh #4579: Optimized dashboard stream query
- Enh #4579: Optimized live legitimation id queries
- Enh #4579: Added `dashboard\Module::$guestFilterClass` and `$memberFilterClass` to replace dashboard filter class
- Enh #4586: Rebuild group default Space Mapping
- Enh #4225: Delete open/pending registration invites automatically after a period of time
- Fix #4718: Fix space or profile banner size after crop
- Enh #4738: Allow CanComment permission also on profile level
- Enh #4511: Default group for users who are not assigned to any other group
- Enh #4749: Add Migration helper to determine installation state
- Enh #4611: Added console command to display LDAP attributes of a user
- Enh #4750: OAuth: Automatically link OAuth Account with same e-mail address
- Enh #4706: Marketplace: Possibility to prohibit modules via the configuration
- Enh #4770: Added CLI commands for Professional Edition licence management
- Enh #4752: Added file column `hash_sha1` to avoid caching problems
- Enh #3345: Maintenance mode
- Enh #4751: Hide separator between widgets `LikeLink` and `CommentLink`
- Enh #4751: New `ContentObjectLinks` widget for the detail views of module content
- Enh #4754: Shorten high member numbers
- Enh #4781: Change allowed characters in username
- Enh #4416: Added reply to sub comments
- Enh #4571: humhub/libs/Html::containerLink() now adds a "data-guid" attribute
- Enh #4791: Delay failed login attempts
- Enh #4787: Always enable Space Membership Web Notifications
- Enh #4795: Added support for collapsible form fields
- Enh #4796: Added option to disable PWA/ServiceWorker support
- Enh #4808: Improved richtext styles
- Fix #4752: Fix saving hash of a deleted file from disk
- Enh #4671: Implemented live poll result sharing by BroadCastChannel
- Enh #4829: Renamed account "Security" page and make it optional
- Enh #4818: Added database related checks (Driver, Collation, Table Engine)
- Fix #4831: Validate username by pattern only on change or for new users
- Fix #3662: Encoding issues in mails
- Enh #4686: Implemented richtext converter to following formats: plaintext, shorttext, html, plain markdown
- Enh #4686: Enhanced richtext extension API for convterting and post-processing
- Enh #4686: Added caching mechanism for richtext converter results

1.7.3 (February 26, 2021)
-------------------------
- Fix #4792: Guest access to user profile home page
- Fix #4794: CountrySelect profile field broken
- Fix #4793: Form labels (HForm) are not displayed correctly
- Fix #4569: Prevent double module registration
- Fix #4389: Require to check a checkbox if the profile field is required
- Fix #4281: Update space chooser after following a space
- Fix #2950: Close modal window on click link with url in href
- Fix #3687: Disable profile field type for existing record
- Fix #4819: Fixed some PHP8 issues. (Updated to Yii 2.0.40 / Imagine 1.0+)
- Fix #4825: Ensure unique setting values (Added unique table index)
- Fix #4895: Fix js warning of not loaded module space.chooser
- Fix #4921: Fix ambiguous column status
- Fix #4923: Replace denied characters with underscore in uploaded file names

1.7.2 (January 21, 2021)
------------------------
- Fix #4668: table-responsive tables do not overflow due to default word break style
- Fix #4679: Richtext extension scan does not include full title if title contains a `)`
- Fix #4703: SSO login drops no warning if AuthClient cannot be stored
- Fix #4700: Deep Links from Microsoft Office Documents
- Fix #4714: Use HTTPS protocol for default OEmbed endpoint URLs
- Fix #4727: Nav tabs with data-toggle are styled in link color
- Fix #4649: Success message rendered although password validation failed
- Fix #4717: Repsonsive layout alignment issue on small screens
- Fix #4715: Call to `Content::canArchive()` throws error on global content
- Fix #4744: Banner image orientation not being processed
- Fix #4743: Hide "Like" link when no permission "Can like"
- Fix #4768: Use only letters and digits from Space name for logo acronym (Thanks to @jrckmcsb)
- Fix #3617: Deny slashes in usernames

1.7.1 (November 27, 2020)
-------------------------
- Fix #4612: Dashboard wall stream entry displays user name in sub title in post style layout
- Fix #4614: Profile Image crop broken
- Fix #4607: Changed grid size of image preview on fluid themes
- Fix #4609: Error on downscale command
- Fix #4621: Wrong image orientation on downscaling with imagick
- Fix #4628: Fixed stream gallery ratio issues on fluid themes
- Fix #4636: Jplayer overflow on mobile stream
- Fix #4591: Registration error text "You are already logged in!" not translatable
- Fix #4630: Transfer default content of user approve/decline email to approve/decline form
- Fix #4650: `adminCanChangeUserProfileImages` option has no effect
- Fix #4660: Topic stream filter leads to stream entry duplication in combination with stream suppression
- Fix #4638: Profile settings do not accept birthdate in russian format
- Fix #4596: Set `autocomplete="off"` on date picker fields
- Fix #4666: Richtext attachment of multiple files without title fails

1.7.0 (November 4, 2020)
------------------------
- Fix #4590: Page loader color contrast too low
- Fix #4599: File preview not visible if initialized in background

1.7.0-beta.2 (October 26, 2020)
-------------------------------
- Fix #4504: Fix `hasSidebar()` for empty sidebar
- Fix #4526: `HeaderControlsMenu::init` called twice
- Fix #4529: Aligned default dropdown text size
- Fix #4533: Removed "Can Like" permission from permission settings for "Not registered users"
- Fix #4534: In profile checkbox field, `Other:` not translatable
- Fix #4547: Fixed wall stream entry header title text style
- Fix #3980: Empty stream on permalink for content a user is not allowed to access
- Enh #4448: Exclude all media preview files from file list if `excludeMediaFilesPreview` setting is active
- Fix #4542: Ignore displaying `Member Since` for empty created_at membership
- Fix #4549: Handle invalid timezone validation in registration process
- Enh #4531: Remove wall entry left padding on mobile
- Fix #4554: Code blocks in comments uses same background color
- Fix #4574: Different style between clickable and non clickable space/user counter
- Fix #4575: Increased text size of "Read more" link on short-text post
- Fix #4575: Increased text size of "Read more" link on short-text post
- Fix #4559: Don’t check platform php extensions by composer v2
- Fix #4581: Users see content of archived spaces on dashboard

1.7.0-beta.1 (October 16, 2020)
-------------------------------
- Fix #4327: Internationalization of user approval/decline message text
- Fix #4139: Dashboard post input on mobile cuts editor menu
- Fix #4328: Top navigation overlaps post input richtext menu on dashboard page
- Fix #4257: Notification dropdown text breaks after notification image on mobile
- Enh #4341: Simplified console controller map
- Fix #4272: Guess timezone for new accounts
- Fix #4230: Auto enable "Hide file info (name, size) for images on wall" option
- Chg: Move CHANGELOG to humhub root
- Fix #4330: Allow users with permission ManageUsers to modify profile images
- Enh #4179: Removed deprecated mysql character set in log table migration
- Enh #4324: Improved line break for menu entries with many characters
- Enh #4186: Add Timezone validation rules to admin prerequisite view
- Enh #4378: Implemented generic ContentContainerActiveRecord::is() function
- Enh #4310: Add "Can Like" Permission
- Fix #4111: Issues Cropping Images
- Enh #4283: Implemented UserMemberSince and UserLastLogin user's profile virtual fields
- Fix #4385: Tour broken when profile start page is changed
- Enh #3882: Rework of wall stream entry widget design and API
- Enh #3882: Introduction of alternative `WallStreamModuleEntry` widget for collaborative content types
- Chg #4397: Deprecated old wall entry widget and related stream logic (see `humhub\modules\stream\actions\LegacyStreamTrait.php`)
- Fix #4391: ActiveRecord `created_at` and `updated_at` contains invalid value after save
- Chg #4397: Default theme color alignment and new `@link` color variable
- Enh #4419: Implementation of view context http header `HUMHUB-VIEW-CONTEXT`
- Fix #4420: Uncaught Throwable destroys search layout
- Enh #4421: Added `Html::addTooltip()` to add tooltips to an option array
- Fix #4422: Invalid Html semantic in activity stream (`li` wrapped by `a`)
- Enh #4423: Implemented icon alias configuration in ui module class
- Enh #4424: Posts content with short text is emphasized
- Enh #4425: Use of accessibility compatible icon tooltips
- Fix #4408: JPlayer on mobile overflows stream content
- Fix #4382: Use of proper word break style
- Fix #3566: Bug in models/filetype/CheckboxList.php
- Enh #4401: Allow to use less variable name in value of another less variable
- Fix #4434: Fix title quoting for space icons in widget “Member in these spaces”
- Fix #4428: Replace db Expression time now with func date('Y-m-d G:i:s')
- Enh #4370: Add "about" to `Space` model
- Enh #4370: Add `humhub\modules\space\widgets\MyMembership` to manage render user state in a space
- Enh #4370: Add `humhub\modules\space\widgets\AboutPageSidebar` to manage about page sidebar
- Enh #4370: Add `About Space` page
- Fix #3994: Live event legitimation array include followed users
- Fix #3994: Live event legitimation consider `cached` argument in processing data
- Fix #4452: `humhub.ui.filter.getActiveFilterCount` returns wrong value with exclude array option
- Fix #4452: Ignore `scope` profile filter in stream filter count and hasActiveFilters
- Fix #4456: PHP8 deprecated warning for LessHelper::updateVariables()
- Fix #4451: PHP Deprecated Warning in ProsemirrorRichText::replaceLinkExtension
- Enh #4195: Increased scaled logo size for high res displays
- Enh #4469: Added TextConverter maximum length
- Enh #4469: Added file converter id attribute
- Enh #3978: Added option to compress and resize images automatically on upload
- Enh #3889: Prevent automatically resized site icons by manually added files (e.g. `/upload/icon/180x180.png`)
- Enh #4458: Remove cacert.pem in order to avoid curl error
- Enh #4467: Inject stream entries by event (experimental)
- Fix #4473: Catch all Throwables when loading module configuration
- Fix #4474: Loader not removed from event trigger
- Enh #4476: Reworked TimeAgo widget
- Chg #4482: Removed old legacy richtext editor which is deprecated since v1.3
- Enh #4475: Add Console UserAdmin Command
- Chg #4482: Removed old legacy richtext editor which is deprecated since v1.3
- Enh #3851: Migrate components from ZendFramework to Laminas
- Fix #4354: Set `about` as target url of space invitation notification
- Fix #4493: Removed legacy ControllerAccess in notification ListController
- Chng #4509: Removed `humhub\modules\space\widgets\Picker` which is deprecated since v1.2
- Fix #4396: Submitting only picture in comment results in debug error.
- Enh #4469: Added alias for file uploads folder
- Fix #4513: Make like counter clickable in first like

1.6.5 (Unreleased)
------------------

- Fix #4555: Default password validation error message missing translation and wrong min. characters
- Fix #4494: Empty "Add Modules" step on space creation when all modules are always enabled

1.6.4 (October 9, 2020)
-----------------------

This release also brings a [security update](https://github.com/yiisoft/yii2/security/advisories/GHSA-699q-wcff-g9mj) of the Yii2 framework. HumHub itself and the modules provided by our offical marketplace are not affected by this bug.

- Fix #4361: Added missing nonce attribute in inline marketplace script
- Fix #4363: Open file modal throws permission denied for unauthenticated users in guest mode
- Fix #4371: Word break issue in notification dropdown
- Fix #4355: Fixed error when authclient not providing an id attribute
- Fix #4384: Upgrade to Yii 2.0.38
- Fix #4403: Space Picker Double HTML Encode
- Fix #4385: Tour broken when profile start page is changed
- Fix #4430: Invalid notifications breaks notification overview

1.6.3 (September 9, 2020)
-----------------------
- Fix #4315: UserInvite (E-Mail Approval) not deleted when declining users
- Fix #4318: Timezone issue with LDAP and birthday fields
- Fix #4331: Directory pageSize module option has no effect
- Fix #4333: Marketplace download of beta versions broken
- Fix #4342: Missing Emoji mappings used for plain richtext output
- Fix #4343: Autofocus of picker input in modal not working
- Fix #4323: TabbedForm validation switches to erroneous tab on every client form validation

1.6.2 (August 4, 2020)
-----------------------
- Fix #4305: 2nd level comment "Submit" button not visible

1.6.1 (August 3, 2020)
----------------------
- Fix #4282: Sub-comment richtext menu dropdown does not hover main comment section
- Fix #4285: All ThirdParty modules are also marked with "Community"
- Fix #4287: Fixed Yii2 compatibility issue with MySQL 8+
- Fix #4303: Fixed syntax error in comment query

1.6.0 (July 29, 2020)
---------------------
- Fix #4256: MOV file support broken with wrong MIME Type
- Fix #4274: Force profile field attribute values of BaseTypeVirtual fields
- Fix #1438: Error "User or Password incorrect." not translatable
- Fix #4262: Additional hr in comment section
- Fix #4161: Number of "n more" likes is invalid

1.6.0-beta.1 (July 16, 2020)
----------------------------
- Enh: Improved performance of cli marketplace module updater
- Fix #4054: Duplicate "font-weight" value
- Enh: Prevent 100% image height in blueimp gallery
- Chg #4170: Updated codeception to v4.1.6
- Chg #4138: Updated jQuery to v3.5.1
- Chg #4158: Cleanup post table removed unused column
- Fix #4182: Native edge password reveal icons interferes with custom one
- Fix #4173: Notification overview HTML compliant issue
- Enh #4191: Added SortOrder Form Input Field
- Enh: Added `ContentVisibilitySelect` ActiveField widget for content forms
- Enh #4213: Only render topic chooser if there are topics available or user can create topics
- Enh: Added `humhub\modules\ui\form\widgets\ActiveField:preventRendering` to manage render state within field classes
- Enh: Added `humhub\modules\ui\form\widgets\JsInputWidget:emptyResult()` helper to manage render state of JsInputWidget
- Enh: Added `humhub\modules\ui\form\widgets\JsInputWidget:field` in order to access ActiveField instances within JsInputWidget
- Enh #4216: Added `humhub\modules\ui\filter\widgets\DropdownFilterInput` in order to support dropdown stream filters
- Enh: Added support for non-free marketplace modules without a fixed price
- Enh: Show more information about installed module in marketplace when possible. Instead of limited README.md
- Enh #3923: Add ability to disable profile stream
- Enh #4222: Added virtual profile fields to display users e-mail address and username
- Enh #4194: Increased max pinnable space content
- Enh #4194: Make max pinnable content configurable on space/profile level
- Chg #4228: Removed unnecessary `ContentActiveRecord:initContent`
- Fix #4229: `Space::canAccessPrivateContent()` throws error for guest user if `globalAdminCanAccessPrivateContent` setting is true
- Fix #4227: Removed redundant code from `humhub.ui.widget.js`
- Fix #4232: Metadata request creates guest session if CSP nonce header is enabled
- Enh #4234: Enhanced custom test environment configuration in `@protected/humhub/tests/config/env/env.php` file
- Fix #4233: `humhub\modules\web\security\helpers\Security:setNonce()` does not remove nonce session value if nonce is null
- Fix #4235: Misleading error message 'Unable to determine dataType from response' logged on ajax error
- Enh #4238: Added module marketplace option for Community Modules. Updated third-party Module disclaimer
- Enh #4238: Added module marketplace option to enable module beta version updates
- Fix #4199: Pinned posts of other spaces are excluded from profile stream
- Enh #3995: Added additional user profile stream filter to include or exclude non profile stream content
- Enh: Added `humhub\modules\stream\actions\Stream:initQuery` to manage query filter in subclasses
- Enh: Make profile content archivable
- Enh: Archived stream filter now only included archived content

1.5.3 (July 16, 2020)
---------------------
- Fix #4036: Profile images are not rotated correctly
- Fix #4168: Erroneous pagination in notification overview
- Fix #4060: Profile description and text regex error message not translatable
- Fix #4153: Administration: Email transport configuration 'Save & Test' Gives No Result
- Fix #4187: Use of invalid LivePushAsset namespace
- Fix #4140: Profile field hint is double encoded
- Fix #4166: Typo in LDAP settings form

1.5.2 (May 20, 2020)
--------------------

- Fix #4031: Notifications with non existing base model breaks notification list
- Fix #4038: Cannot use yii\helpers\Html as Html because the name is already in use in ProfileBannerImage
- Fix #4050: Broken Cron-job documentation link used in cron info sidebar snippet
- Fix #4036: Uploaded photos are not rotated correctly
- Fix #4078: Richtext linkextension pattern fails on link extensions with containing `)` in link title
- Fix #4080: Invalid absolute urls created in acceptance tests
- Fix #4030: #search-menu-nav required in theme view layout main
- Fix #4086: Maximum call stack size exceeded thrown on ActivityStreamEntry.remove
- Enh #4088: Improved table overflow handling in richtext content
- Chg: Updated humhub richtext version to 1.0.25
- Fix #4091: Richtext compatibility parser translates links within code blocks
- Fix #4096: Missing CreatePost permission check in post model canMove
- Fix #4098: Space setting edit fails due to unique name validation
- Fix #4100: Empty message validation errors on post and comment edit broken
- Enh #4061: Improved post context menu order
- Fix #4056: Images not rendered in markdown profile field
- Fix #4034: Premission filter pagination shown without reason and broken
- Fix #4012: Permission filter dropdown shows module id instead of module name
- Fix #4046: Search results not highlighted
- Fix #3975: Space chooser directory button visible, even if user is not allowed to access directory
- Fix #4106: Profile about displays birthdays in current user timezone
- Fix #4108: Issues deleting network logo
- Fix #4119: Oembed not found due to different encoding
- Fix #4084: Blueimp gallery image assets not published
- Fix #4069: Duplication of log level filter parameter in pagination url
- Fix #4075: Use of array_key_fist in space CreateController fails on PHP < 7.3
- Fix #4033: Checkboxlist profile field does not support `Key => Option` format as described in help text
- Fix #4125: See password field addition calculates wrong position with container animation
- Fix #4127: Richtext fullscreen mode within modal or login-container broken
- Fix #4116: Definitive user deletion doesn't work

1.5.1 (April 19, 2020)
----------------------

- Fix #4001: LDAP user sync error
- Fix #4004: Missing translation strings
- Fix #4009: Yii queue error handling broken
- Fix #4008: Some richtext images are embedded as Base64
- Fix #4019: Animated Gifs not handled correctly with GMagick extension
- Fix #4021: Activity mail queue job timeout error handling
- Fix #4005: The uploaded logo is scaled too small.
- Enh #4026: Check memory limit in prerequisites check
- Fix #4023: Background flickering on firefox page transition
- Fix #4028: Image previews rendering in stream do not perform well.

1.5.0 (April 15, 2020)
----------------------

- Fix #3976: User profile stream could not be initialized
- Fix #3977 Reverted nicescroll version to 3.6.6 due to mobile scroll issues
- Chg: Only use nicescroll on space chooser, notifications, and activity stream on large devices
- Chg: Replaced `humhub.ui.view.isNormal()` with  `humhub.ui.view.isLarge()`
- Fix #3973: Profile Categories Not Editable
- Fix #3925: "Back to stream" button visible after pin to top in stream
- Chg: Removed all style assets from CoreBundleAssets
- Fix #3991: Archive content triggers "New updates available" stream badge

1.5.0-beta.1 (April 6, 2020)
----------------------------

- Enh #3858: Support SameSite cookies
- Fix #3861: Improved warning details when auto delete inconsistent notification
- Fix #3873: Invalid visibility handling in `Content::canView()` for private global content
- Fix #3896: Top menu dropdown double border on focus/hover
- Fix #3834: Many entries in the top menu crashing layout
- Enh #3907: Allow `client.ajax().abort()`
- Enh #3909: Add filters to `Administration -> Information -> Logging`
- Enh #3910: Add javascript url util `humhub.util.url.getUrlParameter()`
- Enh #3557: Add permission filter to space and user permission settings
- Enh #3844: Add directory menu icons
- Enh #3792: Render profile field description as form hint
- Enh #3841: Allow * as group-id in `defaultPermissions` configuration
- Enh #3924: Implement `StreamQuery->$to` field and query for stream updates
- Enh #3927: Add `content.container.guid()` function to determine active container on the frontend
- Enh #3924: Display update stream badge once an update is available
- Enh #3924: Implement `Stream.isUpdateAvailable()` to determine if there is an update available
- Enh #3924: Implement `Stream.onUpdateAvailable()`, `Stream.loadUpdate()` and `Stream.options.autoUpdate` to manage stream updates
- Enh #3924: Added `humhub\modules\content\live\NewContent:$streamChannel`
- Enh #3928: Implement auto updates on activity stream
- Enh #3930: Add default `Stream.initScroll` with support of IntersectionObserver
- Fix #3904: Removed unused "alt" attribute on Span element
- Enh #3950: Include non profile content to users profile timeline
- Enh #3937: Add test mail to mail settings
- Fix #3912: Unneeded inline style breaks stylesheet in logo.php
- Enh #3402: Replaced ImageConverter class with Imagine
- Enh #3939: Add `client.redirect` action to client js module
- Enh #3941: Core asset bundle optimization
- Enh #3428: Added dashboard stream filter
- Fix #2456: Only display list of relevant modules on space creation (@armezit)
- Fix #3954: Support LDAP servers without pagination
- Enh #3958: Mark legacy modules in module overview
- Chg: Added gradient to `ui.showMore` feature
- Chg: Removed legacy `humhub\assets\PagedownConverterAsset` from AppAsset
- Chg: Removed legacy `humhub\assets\JqueryCookieAsset` from AppAsset
- Chg: Removed legacy `resources/file/fileuploader.js` from AppAsset
- Chg: Removed legacy `resources/user/userpicker.js` from AppAsset
- Chg: Removed legacy `js/humhub/legacy/jquery.loader.js` from CoreApiAsset
- Chg: Removed legacy `js/humhub/legacy/app.js` from CoreApiAsset
- Chg: Removed legacy `js/humhub/humhub.ui.markdown.js` from CoreApiAsset
- Chg: Deprecated `humhub\modules\ui\form\widgets\MarkdownField` in order to favor `humhub\modules\content\widgets\richtext\RichTextField`
- Chg: Use lazy js module fallback for `humhub.require()` by default
- Chg: Only register live push asset and `SocketIoAsset` on demand
- Chg: Updated Yii2 Queue Extension to v2.3.0
- Chg: Migrated from Zend Http to Yii2 HttpClient
- Enh #3916: Rework profile field administration overview
- Fix #3635: Search rebuild job timeout
- Fix #3965: Space deletion not possible on some AuthClients without password
- Chg: Replaced Space archive and Space delete buttons
- Fix #3813: Too high memory consumption on Notification cleanup
- Chg: Updated richtext version to 1.0.22

1.4.5 (Unreleased)
------------------
- Fix #3945: Default object-src policy prevents loading pdf on safari
- Fix #3963: Richtext/Markdown links not highlighted by default
- Fix #3986: Cannot use yii\helpers\Html as Html because the name is already in use in `humhub\libs\ProfileBannerImage`

1.4.4 (March 24, 2020)
----------------------
- Fix #3908: `DateHelper::parseDateTime()` returns invalid date if given value is not parsable
- Fix #3905: `accountTopMenu` renders redundant `<li>` tag
- Fix #3911: Error thrown in UrlRule for non existing user names
- Fix #3914: Directory link in space chooser still visible when directory module not active
- Fix #3915: Removed default border from canvas style
- Fix #3885: Prevent comments on archived content
- Fix #3940: Empty visibility for some new spaces
- Fix #3942: Show password icon not placed correctly if field was initially hidden
- Chng: Updated richtext version to 1.0.21
- Fix #3906: Prevent emoji chooser focus when triggered by input rule
- Fix #3890: Richtext list menu item disappears

1.4.3 (March 4, 2020)
---------------------
- Fix #3887: CSS presentation issue for tables wider than the container and videos missing borders (areasas)
- Fix #3893: New user invite headline broken in German translation
- Enh: Updated translation files
- Fix #3894: Pjax call does not does not release scroll body scroll lock when default swipe is active
- Fix #3897: Top menu dropdown on mobile does not update active state

1.4.2 (Februrary 27, 2020)
--------------------------

- Fix #3865: "Use default swipe" setting not working
- Fix #3875: Profile image click does not open gallery overlay
- Fix #3879: New mobile swap interfers horizontal scroll
- Enh: Added `humhub.ui.view.isActiveScroll()` in order to check current scroll state (e.g. used to prevent swipe)
- Enh: Added `humhub.ui.view.preventSwipe()` in order to prevent default swipe
- Fix #3866: Emoji chooser broken after pjax link
- Enh: Added emoji richtext menu item
- Enh: Updated humhub richtext version to 1.0.20
- Fix #3883: Former & soft deleted LDAP user produces multiple warnings

1.4.1 (Februrary 17, 2020)
--------------------------

- Fix #3852: Error when OpenSSL extension is not installed
- Fix #3849: ModuleCleanupJob produces an error due to ".." in path
- Fix #3860: Console/Cli Marketplace actions broken
- Fix #3862: Profile field type checkbox list with multiple values broken
- Fix #3864: Some profile field translations broken

1.4.0 (February 4, 2020)
------------------------

- Fix #3789: TopicPicker `addOptions` flag ignored
- Fix #3790: "Create post" permission visible in profile permissions settings for guest user group
- Fix: `AdminMenu:reset()` fails on console requests using user switch
- Fix: Default `ContentContainerController::subLayout` can't be overwritten directly or within controller `init`
- Fix #3791: Topic overview missing for user profiles
- Fix #3787: Required checkboxlist input shows asterisk on each option
- Chng: Removed `static/temp.css`, moved required form style to `form.less`
- Enh: Use of colored required input field asterisk
- Fix #3784: `ActiveQueryContent::readable()` not working for global content
- Chng: Removed italic text from summary mail of comment and content activities for better readability
- Fix #3798: DBValidator not working with time value and swedish locale
- Enh #3779: Added `ui.view.getContentTop()` for calculating the top position of the layout content with theme support
- Fix #3704: Public space is not displayed when guest user accesses "Space directory".
- Fix: Fixed modal width calculation on mobile (ee)
- Fix: Dropdown width issue on mobile (ee)
- Fix: Prevent sidebar swipe on menu scroll
- Fix #3805: Cannot select more than one activity in E-Mail Summaries settings
- Fix #3802: 'usersearch-status' dropdown triggers reload on click
- Chng #3816: Use of `static::class` query class within `ContentActiveRecord::find()` instead of `getObjectModel()`
- Fix: DBDatevalidator returns unix epoch date when parsing with a time value fails
- Enh: Notification targets can be deactivated or overwritten by configuration
- Fix #3810: Print Media Cluttered by HREF Content
- Enh: Added further print style enhancements
- Fix #3803: Invalid editor preset handling
- Fix #3829: Guest user access to counter set freezes
- Enh: `data-action` url now can be set as `href` attribute additionally to  `data-action-url`
- Fix #3837: Legacy modal may freeze in case of errors
- Fix #3796: Guest users can't access public posts from 'Latest activities'
- Fix #3797: User `humhub\modules\user\widgets\Image` link was disabled by default
- Fix #3795: Open Sans load downloadable font: kern: Too large subtable, table discarded
- Chng: Dropped open-sans npm dependency and updated and included font in `static/css/open-sans.css`
- Enh: Update Yii version to 2.0.32
- Enh #3822 Added content id to notification urls as fallback in case notification was deleted
- Fix: Settings cli rewrite dynamic config when required
- Fix #3806: Using `Receive notifications for new content` will not include the space to the notification setting view until settings are saved
- Enh: Added possibility to disable mail summary feature
- Fix #3848: Error page does not use theme

1.4.0-beta.2
------------

- Fix #3703: Fixed user profile image dimension of mobile
- Fix #3732: Reverted changes of default oembed style
- Enh: Added link to changelog for module marketplaces updates
- Fix #3674: Back button breaks layout on login page when guest access enabled
- Enh: Added `safeCreateTable`, `safeDropTable`, `safeDropColumn`, `safeAddColumn` to `humhub\components\Migration`
- Fixed `.layout-nav-container` padding issue
- Fix #2605: User display name cropped in profile header
- Fix #3729: Integrity check used deprecated methods
- Enh #3697: Stay of module update page after updating a module
- Fix #3692: Icon Upload Problems
- Fix #3705: Don't render empty menus
- Fix #3706: Space mentioning broken
- Fix #3742: OAuth timeout doesn't respect configured timeout
- Enh: Added `DateHelper:getUserTimeZone()`, `DateHelper:getSystemTimeZone()`, `DateHelper:isInDbFormat()`
- Fix #3711: Fullscreen Richtext menu broken on ios safari
- Enh #3768: Add `Module::afterUpdate`, `Module::beforeUpdate` events to `humhub\components\Module`
- Enh: Add `OnlineModuleManager::EVENT_BEFORE_UPDATE`, `OnlineModuleManager::EVENT_AFTER_UPDATE`
- Fix: Double encoding of `&` in `Richtext::output()`
- Enh: Added `SocialActivity::getContentPlainTextPreview()` mainly used in mail subjects
- Enh: Added `data-ui-addition` way of definint ui additions
- Enh: Added `data-ui-addition` way of defining ui additions
- Enh #3771: Added `data-ui-addition="acknowledgeForm"` in order to prevent page changes without save/confirmation
- Enh #3771: Added `humhub\modules\ui\form\widgets\ActiveForm:acknowledge` flag
- Chng: Use of `BlueimpGalleryAsset` npm asset instead of static asset file
- Enh: Updated richtext version to 1.0.18 see (https://github.com/humhub/humhub-prosemirror/blob/master/docs/CHANGELOG.md)
- Enh: Added mobile swipe in order to show sidebar (needs to be activated `Administaration -> Settings -> Appearance`)

1.4.0-beta.1
------------

- Enh: GroupPermissionManager - allow to query users by given permission
- Enh: Automatic migrate DB collations from utf8 to utf8mb4
- Enh: Added Icon widget as wrapper class
- Enh: Moved from bower to npm assets
- Chng: Removed `jquery-placeholder` asset and dependency
- Chng: Removed `atwho` asset and dependency
- Cnng: Removed old IE support
- Fix #2946: Use Yii2 default timezone handling
- Enh: Use LocalStorage in panel menu
- Chng #2164: Removed MSN & Google+ social bookmarks during setup
- Enh: Added a user module configuration for setting password strength rules (Baleks)
- Fix #3103 Password recovery links pjax layout issue
- Enh: Added `humhub.ui.widget.Widget.loader()` for default loader functionality
- Enh: Added `humhub.ui.widget.Widget.reload()` in combination with `humhub\widgets\Reloadable` interface
- Enh: Implemented an auto loading mechanism for notification filters (Baleks)
- Enh: Modules can add or overwrite oembed providers by means of `humhub\models\UrlOembed:EVENT_FETCH` event (Baleks)
- Fix: `WallEntry::EVENT_AFTER_RUN` event not triggered
- Enh: Added `humhub\components\Widget::widgetLayout`
- Enh: Added an option for user to change username (Baleks)
- Enh: Added warning confirmation when module is being deactivated from console (Baleks)
- Enh: Moved 'Default spaces' setting from Basic settings to Space settings (Baleks)
- Enh: Add inviter name to Space Admin Member section (Baleks)
- Fix #3463 Changed 'Deny Invite' to 'Decline Invite' for space invites (Baleks)
- Enh: Responsive mobile view enhancements
- Enh: Added `humhub\widgets\Link::target()` and `blank()`
- Fix: `humhub.client` does not resolve promise on 302 redirects
- Enh: Separated marketplace methods into own submodule
- Enh: Added consistent user "sub" display-name handling
- Enh: Added possibility to manage database settings via CLI
- Fix: Force redirect to login instead 404 when guest access is disabled (thanks to Security Research Team, Datafarm Co.,Ltd.)
- Enh: Added "web" submodule for web specific features (e.g. security headers or PWA)
- Enh: Added Progressive Web App (PWA) support
- Enh: Added integrated page icon handling
- Enh: Raised minimum PHP Version to 7.1
- Chng: New Menu and MenuEntry rendering
- Enh: Added Icon abstraction `humhub\modules\ui\icon\widgets\Icon`
- Enh: Added `humhub\libs\Html::addPjaxPrevention()` for link options
- Enh: Added obj support for `humhub\libs\Sort`
- Enh: Reorganized WallEntry context menu
- Enh: Added new configurable security module with nonce script support
- Chng: Updated jQuery version to 3.4.0
- Enh: Added `humhub\modules\user\controllers\AuthController::EVENT_AFTER_LOGIN` triggered after login success response is rendered
- Enh: Make sure embedded video controls are enabled
- Fix #3404 Richtext `Heading` text not translatable
- Fix #3642 Welcome tour not using community name
- Chng: Moved collapsible panel logic into own js module
- Enh #3649: Provide a way to S/MIME sign e-mails (@ChadiRachid)
- Fix `humhub\modules\file\widgets\Upload::progress` config options not working
- Enh: More generic approach to determine themed view files
- Enh: Always use ISO 639-1 alpha-2 (and ISO 3166-2) language codes
- Enh: Reorganized translation method categories to reduce language files
- Enh: Removed deprecated methods/classes since v1.1 - see migration guide for details
- Enh: Show registration form captcha per default
- Enh: Added abstract `ContentContainerActiveRecord::getDisplayNameSub()`
- Enh: Allow `humhub\modules\files\widgets\Upload::withName($submitName, $cfg);`
- Enh: Auto add `data-container-id` to Space and User `Image` widget
- Enh: Added `grunt test --debug` option
- Fix #3653: Add PHP LibXML requirement
- Enh: Added show password feature for password form elements
- Fix: `humhub\components\acces\AccessValidator` now returns http code `401` for guest and `403` for users by default
- Enh: Added generic `humhub\modules\ui\helpers\models\ItemDrop` model for drag/drop reordering
- Enh: Added `ContentContainer::findRecord($guid)` for loading a ContentContainerActiveRecord by guid
- Enh: Implemented `ProfileImage::render($width, $cfg)` for e.g. `$container->getProfileImage()->render(400)`
- Enh: Added `ContentTag::sort_order` field to provide a default order mechanism for content tags
- Enh: Added `sort_order` configuration for topics
- Enh #3564: Link MemberAdded activity to new member instead of the space
- Enh: Added `humhub.modules.ui.form.submit` action e.g. `data-action-change="ui.form.submit"`
- Chng: Added `humhub.ui.form` namespace to core api asset
- Fix #3567: Profile field type Checkbox List with comma in option list not working
- Enh: Added `changed` and `resetSearch` js widget events to `humhub.space.chooser.SpaceChooser`
- Enh: Added a way to specify script urls, which should not be reloaded (`yii.reloadableScripts`) by configuration and event
- Enh: Add base provider url as `data-oembed-provider` attribute to oembed container
- Fix #3547: Invalid font-family in system mail
- Chng: `humhub\compat\CActiveForm` and `humhub\compat\CHtml` is now deprecated
- Enh: Updated to twemoji v12
- Enh: Editable `['twemoji']['path']` config parameter
- Enh: Added configuration option to hide/disable the Like module
- Enh: Added link to changelog for module marketplaces updates
- Fix #3674: Back button breaks layout on login page when guest access enabled
- Enh: Added `safeCreateTable`, `safeDropTable`, `safeDropColumn`, `safeAddColumn` to `humhub\components\Migration`
- Enh: Added support of upcoming HumHub Professional Edition in Marketplace module
- Enh: Added module marketplace categories
- Enh: Added isFluid LESS variable for automatic HTML container handling
- Fix #2605: User display name cropped in profile header
- Enh: Updated Yii to 2.0.30

1.3.21 (Unreleased)
-------------------
- Fix #3846: Timeline sort by "update" looses entries

1.3.20 (January 9, 2020)
------------------------

- Fix #3814: File uploads broken with restricted file extensions
- Enh: Added `withTimeZone` parameter to `humhub\libs\TimezoneHelper::generateList()`
- Chng: Remove offset information in `humhub\widgets\TimeZoneDropdownAddition` by default

1.3.19 (December 20, 2019)
--------------------------

- Fix #3759: Allow individual file extensions (e.g. msg)
- Fix #3147: Module related permissions are not properly removed on deactivate/uninstall
- Fix #3740: Profile field type Checkbox List does not show "other"
- Fix #3484: Encoding issue in german space visibility translation
- Fix #3717: Account deletion incomplete if related to an identity provider
- Fix #3800: Birthday "Hide year in profile" inconsistent with LDAP

1.3.18 (November 22, 2019)
--------------------------

- Fix #3698: Approval by group manager broken
- Enh: Set max signs of User tags to 250
- Fix: https://github.com/humhub/humhub-modules-wiki/issues/103 Topic attachment fails with given topic instances
- Fix #3366: Set max-width for stream entry image file attachments
- Fix: `ContentContainerController::getAccess` uses `ContentContainerControllerAccess` also for global access
- Fix: Global content does not allow guest access
- Fix #3727 Bug with Bluebird and Firefox 71 breaking mentioning requests

1.3.17  (October 17, 2019)
--------------------------

- Fix #3690: Rollback from broken version 2.8.6 to 2.8.1 of bower-asset/clipboard.js

1.3.16  (October 17, 2019)
--------------------------

- Fix #3647: GroupID field is not translatable in Registration Form
- Fix #3655: Fix CommentLink widget Comment class usage conflict
- Fix #3638: Update Notification Causes System Warning
- Fix #3512: Broken error handling if SQL mode cannot be switched
- Fix #3599: Removed HTML encode for FROM attribute of Email (@githubjeka)
- Fix #3637: Allowed using apostrophe in filename (@githubjeka)
- Fix #3602: Trim function for username (@githubjeka)

1.3.15  (August 22, 2019)
-------------------------

- Fix #3587: New user tour broken on some template variants
- Fix #3589: Reduced integrity check memory usage in Like/Comment module
- Fix #3595: LDAP config file values ignored
- Fix #3598: Removed Google+ default profile field
- Fix #3552: Updated to Yii - AuthClient 2.2+ library
- Fix #3588: OEmbed CSS class not provided
- Fix #3609: LDAP paging control limits max. users
- Fix #3618: Some LDAP CLI commands requires a authClientId parameter
- Fix #3625: If user is following a space of which he is also a member, it shows up twice under "my spaces"
- Fix #3626: SimpleStream reloads unexpected

1.3.14  (June 26, 2019)
------------------------
- Fix: LinkedIn API call to v1 deprecated use v2 (@Felli)
- Fix #3531: File module Fil: isAssignedTo method broken
- Fix: Added missing admin group title encodings
- Enh: Added featured module flag to marketplace view
- Fix: Directory stats progress color (@Felli)
- Fix #2724: Edited post does not display the space on dashboard
- Fix #3533: Responsive design issues
- Fix #3471: Display of Date Time Column in excel with empty/false value
- Fix #3581: Search form with GET causes repeated sticking of url parameters (@Bhoft)
- Enh: Added configuration option to hide Activity sidebar widget on dashboard
- Fix #3570: en-GB language code Datepicker 404
- Fix #3584: "Array to string conversion" on some LDAP attributes
- Fix #3437: Composer warning for bower-asset/jPlayer

1.3.13  (May 3, 2019)
----------------------
- Enh: Added HomeUrl support to ConsoleApplication
- Fix #2536: Incorrect log of "Attempt to steal file" due to faulty File::isAssignedTo() check
- Fix: Wrong help block position in admin basic settings
- Chng: Removed yiisoft/yii2-apidoc dependency
- Enh: Double file extension check is now optional and disabled by default
- Fix #3552: `humhub\modules\user\authclient\AuthAction:auth()` not compatible with `yii\authclient\AuthAction:auth()`
- Fix #3545: OEmbed fetch limit ignored
- Enh: Added `humhub\libs\RestrictedCallException`
- Chng: Switched from [bootstrap-tour](https://github.com/sorich87/bootstrap-tour) to [bootstrap-tourist](https://github.com/IGreatlyDislikeJavascript/bootstrap-tourist) due to incompatibility to bootstrap v3.4.1
- Enh: Added `humhub.modules.tour` module for handling tour logic
- Fix: Added PHP 7.3 compatibility workaround for ZF2 ArrayObject
- Fix #3513: Profile schema cache not refreshed after adding new profile field
- Fix: Removed Codeception files from HumHub packages builds due to possible XSS flaw (thanks to Kağan Eğlence)
- Fix #3534: Mark ID Attribute in LDAP settings as required
- Fix #3662: Group picker encode issue

1.3.12  (March 26, 2019)
---------------------------
- Enh: Use of new Richtext for About section
- Chng: Force blank links in old markdown editor
- Fix: Profile Markdown field files are not attached
- Chng: Don't restrict`humhub\modules\file\components\FileManager::attach()` to `humhub\components\ActiveRecord`
- Fix: Richtext preview new line backslash issue
- Enh: Migrated LDAP features into own submodule
- Enh: Added new LDAP command line tools
- Fix #3347: Fixed searching members in space and users with white space in full name (Baleks)
- Fix: Deleted Records are not correctly removed from the search index
- Fix #3459: Notification counter increment after manual notification fetch
- Fix: Notification count update does not respect notification group
- Fix: Change email form is restricted to max 45 characters. Changed to 150 (current DB restriction)
- Fix: Footer menu renders redundant `<li>` end tag.

1.3.11  (March 06, 2019)
---------------------------
- Fix: Disabled module notification category visible in notification settings.
- Enh: Added `ModuleManager::getEnabledModules()`
- Enh: `LikeAsset` is now part of `AppAsset` and does not need further registration
- Fix (CVE-2019-9093) and (CVE-2019-9094): Reflective XSS in file post upload and cfiles upload (thanks to **Rubal Jain** for testing and reporting)
- Enh: Added further upload file name validation
- Enh: Added `ContentContainerModuleManager::flushCache()`
- Fix: Bootstrap modal blocks richtext prompt focus
- Fix: Richtext images with dimension setting not attached
- Fix: `Stream::renderEntry()` overwrite does not work
- Fix: Removed markdown line breaks from richtext preview
- Fix: WallEntry of global content throws error
- Fix: `ActivityAsset` does not depend on `StreamAsset`
- Fix: Uploaded png preview files lose transparency
- Fix: Modal options `backdrop` and `keyboard` deactivation has no effect

1.3.10  (February 22, 2019)
---------------------------
- Fix: Removed ContentTag logging in search update
- Fix #2567 No results in directory search containing single quote ( ' )
- Fix #3468 Private space stream contains public content filter
- Fix #3473 Captcha validation breaks invite by mail
- Enh: `data-action-confirm` now works on non action based links in combination with `data-action-method`
- Enh: `grunt test` now uses the composer codeception version instead of a global executable
- Enh: `grunt test` supports an additional `--env` option in order to set the codeception environment
- Fix: Absolute url generation in tests not working
- Enh: Added `HumHubHelper:fetchinviteToken()` in order to fetch invite tokens from emails in functional tests
- Fix: Added "utf8mb4" character set support to database requirements
- Fix: Finnish language name in language dropdown

1.3.9  (February 13, 2019)
--------------------------

- Fix: StreamSuppressedQuery with limit = 2 throws query not executed exception
- Fix #3378: Update user in search index when group memberships changes
- Fix: Space un-archived activity view path broken
- Enh: Accepting module README.md files in 'docs' directory
- Fix: Include user profile posts option in dashboard stream broken
- Fix: Check SoftDeleted user state in ControllerAccess
- Fix: Removed database charset configuration in dynamic config
- Fix: User soft deletion membership cache overwrite
- Fix #3422 Stream suppressed loading logic loads unnecessary stream entries
- Fix: "Back to home" button in registration broken with user approvals and guest mode activated
- Fix #1683 #553: Added link to show/edit users awaiting admin approval
- Fix: TextFilterInput uses `keypress` event instead of `keydown`
- Fix #3452: Soft deleted user remain in other users as friends
- Fix #3170: Wrong cancel invitation mail handling
- Enh: Added `humhub\modules\space\models\Membership::isCurrentUser()`
- Enh: Added `humhub\widgets\Link::post()` for `data-method="POST` requests
- Fix: Use `humhub\modules\user\components\ActiveQueryUser::active()` on UserPicker fillquery by default
- Added `relativeUrl` to notification view parameter
- Fix #3335: Queue migration broken on some database configurations
- Enh: Added new admin setting "Include captcha in registration form"
- Enh: Added contentTags to the search index

1.3.8  (December 10, 2018)
---------------------------

- Fix #3359: Weekly summary e-mails are not sent in default configuration
- Fix #3365: Legacy richtext emojis not parsed in richtext preview
- Fix: Friendship button adds additional spaces
- Fix: SpaceController::actionHome throws 403 Http error for guests
- Enh: New `humhub\modules\user\components\User::EVENT_BEFORE_SWITCH_IDENTITY`
- Fix: Administration menu item visible after user impersonation
- Enh: Added PermissionManager findUsersByPermission feature

1.3.7  (October 23, 2018)
---------------------------

- Enh: Added maximum username length & maximum/minimum space url length (rekollekt)
- Fix: Error message during database installation
- Enh: "Powered by" message handling by widget
- Enh: Add less options for mail font url/family (@rekollekt)
- Fix: Fixed typo in space (un-)archived activities
- Enh: Removed ErrorEvent which will be removed in yii-queue 3.0 (@acs-ferreira)
- Enh: Added config option to remove "user profile posts" entry from directory navigation
- Fix #2912: Deleting single stream item does not reload stream
- Fix: Updated blueimp/jQuery-File-Upload to 2.94.1

1.3.6  (October 11, 2018)
---------------------------

- Fix: Richtext loses mark state
- Fix: New comment scroll behavior not used in edit comment
- Chng: Updated `humhub-prosemirror-richtext` to v1.0.12
- Fix #3322: Disabled users still receive emails notifications

1.3.5  (October 10, 2018)
---------------------------

- Fix: Serialization of notifications without originator fails
- Fix: Hide unapproved member activities
- Fix #3313: Unable to deny invitation to private space
- Fix: Added missing `parent::init()` to `humhub\modules\stream\widgets\StreamViewer`
- Fix: Added PHP GD extension to the requirements (docs and selftest)
- Fix: Comment edit triggers new activity
- Fix: Fixed typo from `MailSummary::INTERVAL_HOURY` to `MailSummary::INTERVAL_HOURLY`
- Enh: Added `humhub.modules.ui.filter.TextInput` and related `humhub\modules\ui\filter\widgets\TextFilterInput`
- Enh: Enable `data-action-keypress` by default
- Enh: Added `preventDefault` argument to `humhub.modules.action.bindAction` to disable prevent default behaviour for action events
- Fix: Fix bootstrap-datepicker.en.min.js 404 (Not Found)
- Fix: Comment form files not cleared
- Enh: Added `humhub\modules\file\models\isAssignedTo($record)` argument in order to check if a File is attached to a specific record
- Fix: rich-text mobile view wrong min-height calculation
- Fix #3314: layout container width differences
- Fix #3315: Exception on first login with ldap
- Fix comment scroll overflows button
- Fix widgetAction events case issue
- Added `humhub.modules.util.string.capitalizeFirstLetter` and `lowerCaseFirstLetter`

1.3.4  (September 25, 2018)
---------------------------

- Fix: Theme parent lookup cache causes installer crash

1.3.3  (September 24, 2018)
---------------------------

- Fix: img overflow in markdown view
- Enh: Added console command to list and change themes
- Enh: Improved theme parent lookup performance
- Enh: Added auto file attachment in `humhub\modules\content\widgets\richtext\ProsemirrorRichTextProcessor`
- Fix: z-index issue with fixed richtext menu
- Fix #3294: space picker encoding
- Chng: Prevent `ActiveRecord::save()` call in `humhub\modules\file\components\FileManager::attach`
- Fix: Added additional notification validation
- Fix: Notification previews contains new line
- Enh: Allow urls in array form in homeUrl configuration
- Fix: Javascript `humhub.modules.util.object.extend` not working on older Safari version
- Enh: Enable usage of `humhub\modules\content\widgets\PermaLink` outside of `humhub.modules.content.Content` components.
- Fix #3302 smiley are not render into last activity module and email
- Fix: Space head count includes disabled user
- Fix: Broken picker image alignment (acs-ferreira)
- Fix: File handling in upgrade path between 1.0.x and 1.3.x
- Chng: Updated `humhub-prosemirror-richtext` to v1.0.10
- Fix: File handling in upgrade path between 1.0.x and 1.3.x

1.3.2  (September 4, 2018)
--------------------------

- Fix #3241: Profile header space count invalid
- Fix: Disabled Notification E-Mails for installation sample contents
- Fix: No e-mail summary immediately after installation
- Enh: Added queuing for search updates of commments
- Enh: Added queue clear option at Administration - Information
- Enh: Improved support of languages unsupported Yii2
- Enh: Added Amharic language support
- Enh: Added Finnish language support
- Enh: Added dashboard warning for admins if cron jobs not working
- Fix: Queue worker problem with spaces in PHP binary path
- Fix: Comment buttons overlap editor text
- Enh: Added windows support for grunt tasks
- Enh: Added `grunt test-server` and `grunt test`
- Chng: `humhub\modules\content\models\Content` now implements `humhub\modules\content\interfaces\ContentOwner`
- Fix: Target container not available in `humhub\modules\content\components\ContentActiveRecord:afterMove()`
- Chng: `humhub\modules\topic\models\Topic::attach` now accepts `humhub\modules\content\interfaces\ContentOwner` instances
- Fix: Richtext without focusMenu on small devices overlaps previous sibling
- Enh: Added random default color to `humhub\modules\ui\form\widgets\ColorPicker`
- Chng: `humhub\modules\content\models\ContentTag:deleteAll()` and `humhub\modules\content\models\ContentTag:findAll()` now respect the tag type condition by default- Fix: Space admin user remove broken
- Fix: Space admin user remove broken
- Fix: Invalid "Member since" date in space administration
- Fix: Suprressed stream entry button not rendered.
- Fix: Author stream filter not working.
- Chng: Use of relative urls in richtext files/images
- Fix: Permalink better handling of deleted content
- Fix: Activity exception on integrity check
- Fix: Ensure profile field "internal name" contains at least one character
- Fix: Do not allow user self deletion via admin section
- Fix: Refactored ActiveQueryContent::contentTag method, added method parameter
- Fix: Richtext prompt not removed on pjax load
- Enh: Added `humhub\modules\content\widgets\richtext\ProsemirrorRichText::parseOutput` for pre render parsing
- Enh: Added `humhub.modules.file.getFileUrl` and `humhub.modules.file.filterFileUrl` for file guid based url handling
- Fix: `humhub\modules\space\modules\manage\components\Controller` only accessible by system admins
- Enh: Added scheme parameter to Content::getUrl method
- Enh: Added `ui.richtext.prosemirror.config.link.validate` to intercept link input validation
- Chng: Updated `humhub.prosemirror` dependency to 1.0.9

1.3.1  (August 7, 2018)
-----------------------

> Warning: Please read the [Update Guide](http://docs.humhub.org/admin-updating-130.html) before updating from 1.2.x!

> Note: A full list of changes is available here: [Changelog](https://github.com/humhub/humhub/blob/v1.3.1/protected/humhub/docs/CHANGELOG.md)

- Fix: Complete table cache flush on profile field update
- Fix: Improved handling of inconsistent notifications
- Fix: Vietnamese translation syntax error

1.3.0  (August 3, 2018)
-----------------------

> Warning: Please read the [Update Guide](http://docs.humhub.org/admin-updating-130.html) before updating!

- Enh: Added `PolymorphicRelation::strict` to throw exceptions when accessing invalid polymorphic relations
- Fix: Mail summaries not correctly triggered by cron
- Fix: Click to topics lead on streams without topic filter throws javascript error. (https://github.com/humhub/humhub-modules-polls/issues/49)
- Fix: Existing files may cause NULL pointer exception
- Fix: Newly created profile fields cannot be updated
- Enh: Added `AbstractRichTextEditor::layout` in order to change richtext style
- Enh: Added `block` type RichText for non focus menu style

1.3.0-beta.3  (July 30, 2018)
-----------------------------

- Fix: prevent user serialization for SocialActivity
- Fix: wrong return value for `Content::move()`
- Fix: space archive activity wrong originator assignment
- Fix: suppress "unable to determine dataType" error for aborted xhr requests
- Enh: added `FunctionalTester::loginBySpaceUserGroup()` and `FunctionalTest::assertSpaceAccessStatus()` for ACL testing
- Fix #2721 delete space button not visible for system admin
- Enh: added `humhub\modules\space\behaviors\SpaceModelMembership::canDelete()`
- Fix #3221: Popover Space title "&" to "&amp;"
- Fix invalid translation syntax used in croatian language
- Enh added highligh.js as ui addition
- Fix: ui.addition.applyTo with filter ignores first filter index
- Fix: introduction tour not working
- Chng: Moved static js dependencies from `static/resources` into `static/js`
- Fix: Comment edit cancel edit context item not shown
- Fix #2700: Prevent GroupManager access to system admin group management
- Enh: Styled user deletion view
- Fixed: Space and User Admin Filterbar padding
- Fix: Source serialization of Notification ActiveJob
- Enh: Added 'requireSource' & 'requireOriginator' flags in SocialActivities

1.3.0-beta.2  (July 18, 2018)
-----------------------------

Please read the [Update Guide](http://docs.humhub.org/beta/admin-updating-130.html) before updating!

> If you're using the sources directly from GitHub, you need to build the required assets manually. Please see the chapter [Build production assets](http://docs.humhub.org/dev-environment.html#build-production-assets) for more details.

- Enh: Added CounterSet Widget to handle Space/Profile header statistic counts
- Fix: UI addition mutation observer interfering with new rich-text mutation logic
- Fix: ThemeLoader publishes assets on CLI requests
- Enh: Add possibility to delete an invitation [#2980](https://github.com/humhub/humhub/issues/2980)
- Enh: Moved search index tasks (add, update & delete) into asynchronous tasks
- Enh: Added search index rebuild button
- Fix #3200: wall stream scroll not working after single entry load request
- Fix added missing required validation of target space for move content feature
- Enh: Added `humhub.modules.stream.StreamState.firstRequest` in order to determine the initial request
- Fix #3204: invalid russian translation in module overview
- Fix #3169: post markdown not stripped in mails and activities
- Fix #3157: invalid use of relative space target link in MailContentEntry widget
- Fix force invite not working on space creation
- Enh: Enable invite all instead of force membership in case force invite checkbox is not selected
- Fix: prevent MembersAdded activity when using force space membership
- Enh: added `humhub.modules.ui.picker.Picker.disable()` in order to disable/enable userpicker fields
- Enh: topic labels now redirect to space stream with active topic filter if clicked outside of space stream
- Fix: #3123: unbalanced html tags leads to broken comment after load more
- Fix: #3211: escaped html rendered on space list modal
- Fix: invalid userpicker translation syntax in czech language
- Fix: added missing layout-snippet-container class in space and profile layout
- Fix: move profile content not possible
- Fix: Stream wall scroll event not detached on pjax call
- Fix: Error thrown for empty url links in `humhub\libs\Markdown` when used in console environment
- Fix: UserUrlRule double User model import
- Fix: Skip soft delete validation
- Fix: Added user dn to ldap attributes on login
- Enh: Added Twig template engine for usage in modules
- Enh: Added id data attribute on contentcontainer links
- Fix: Wrong permission check on force invite check
- Fix: Space homepage doesn't allow custom pages on first position
- Enh: Added integrity check for notification originator
- Enh: Use of new richtext version 1.0.4 see https://github.com/humhub/humhub-prosemirror/blob/master/docs/CHANGELOG.md
- Enh: Added max-height for post/comment/edit richtext
- Enh: Richtext style enhancements (dashed selection)
- Fix: Upload preview for comments not cleared after submit
- Fix: Profile/Space image upload not working after full page reloads
- Fix: File upload errors not handled by richtext
- Enh: Removed built and compressed assets from GitHub sources

1.3.0-beta.1  (July 4, 2018)
----------------------------

Please read the [Update Guide](http://docs.humhub.org/beta/admin-updating-130.html) before updating!

- Enh: Added file search indexing
- Enh: Updated composer.json (acs-ferreira)
- Chg: Switched from Composer FXP plugin to Asset Packagist repository
- Enh: Committed composer.lock
- Enh: Refactored ContentContainer Controller
- Chg: Added ContentContainer ModuleManager, instead of individual handling (Space/User)
- Fix: Rebind LDAP connection after successful login with administrative user
- Enh: Make utf8_mb4 as default database charset
- Enh: Moved queueing into own submodule and updated to yii2/queue extension
- Enh: Added user soft deletion without contributions
- Enh: Moved user deletion into asynchronous tasks
- Enh: Improved user grid view design (Administration, User Approval, Space Members)
- Enh: Moved SyncUsers (LDAP) and session table cleanup handling into ActiveJob
- Enh: Added Push live module driver using Redis and Node.JS
- Enh: Added tooltip option to space Image widget.
- Enh: Added `humhub.client.json` javascript util for directly receiving json instead of a Response object.
- Enh: Added `humhub.file.Upload.run()` for triggering the upload of the Upload widget.
- Chg: Moved `humhub\widgets\RichText` to `humhub\modules\content\widgets\richtext\RichText`
- Chg: Moved `humhub\widgets\RichTextField` to `humhub\modules\content\widgets\richtext\RichTextField`
- Enh: Added rich text abstraction by means of configuration parameter `richText`
- Enh: Added `humhub\modules\content\widgets\richtext\ProsemirrorRichText` as default rich text.
- Enh: Added `humhub.oembed` js module for loading oembed content
- Enh: Added `RichText::preview()` helper for minimal rich text output
- Enh: Added `RichText::output()` helper for rendering the richtext
- Enh: Added `RichText::postProcess()` for post-processing rich text content (mentionings/oembed etc.)
- Enh: Added `content` module setting `Module::$maxOembeds` for setting the maximim amount of oembeds in a richtext.
- Chg: Deprecate `humhub\modules\user\models\Mentioning::parse()` and in favor of `humhub\modules\content\widgets\richtext\RichText::postProcess()`
- Enh: Added `humhub.user.getLocale()` javascript helper for checking the user locale on client side
- Enh: Added `humhub\widgets\InputWidget::getValue()` for determining the field value
- Enh: Added `humhub.client.json` for directly receiving the json result instead of a response wrapper object
- Enh: Added option ContentContainerController to restrict container type
- Enh: Ensure valid permalinks when URL rewriting is enabled
- Fix: Birthday field refactoring (@danielkesselberg)
- Enh #2811: Added option to resend invites (@danielkesselberg)
- Enh: Added current database name to the "Administration -> Information -> Database" (githubjeka)
- Chg: Depreciated Instagram OAuthClient & removed (@Felli)
- Enh: Added random default space color on creation
- Enh: Updated to Yii 2.0.14.2
- Chg: Reduced email length to 150 chars to support utf8mb4 charset
- Enh: Added UI core module to group UI components
- Enh: Added new IconPicker form field
- Chg: Moved form widgets from `humhub\widgets` to `humhub\modules\ui\form\widgets` (added compatibility layer)
- Enh: Added surpressed e-mail addresses configuration variable
- Chg: `Create a new one.` to `Forgot your password?` (@Felli)
- Enh/Fix: Cache Handling + File Preview Fix (@Felli)
- Enh: BaseSettingsManager allow to bunch delete settings with prefix
- Chg: Migrated view and theme components to  `humhub\modules\ui\view` package
- Enh: Improved Theme component
- Enh: Added notification for MembershipSpace by role member changes (@githubjeka)
- Enh: Added Theme cascading to reduce view overwrites
- Enh: Automatic theme stylesheet loading including parent theme stylesheets
- Chg: Moved OpenSans font to core assets
- Chg: Renamed information cronjob section to Background jobs and added queue status
- Chg: MySQL queue is now the default job queuing driver
- Enh: Add steps to using Facebook Oauth (@Felli)
- Enh: Added css `footer-nav` class for footer navigation
- Enh: Added Pin/Archived/Public wallentry icons
- Enh: Added move content behavior by means of a `humhub\modules\content\models\Movable` interface
- Enh: Added sortOrder utility `humhub\libs\Sort`
- Enh: Added `humhub\modules\content\helpers\ContentContainerHelper` util with `ContentContainerHelper::getCurrent()`
- Enh: Added `humhub\modules\stream\helpers\StreamHelper` util with `StreamHelper::createUrl()`
- Chg: Shifted activity stream logic to `humhub\modules\activity\actions\ActivityStreamAction` and `humhub\modules\activity\controllers\StreamController`
- Chg: Added activity stream action `humhub\modules\activity\actions\ActivityStreamAction`
- Enh: Added `humhub\modules\stream\models\WallStreamQuery` class used for wall streams e.g. Space content stream
- Enh: Added `ui` core module
- Enh: Added abstract ui filters used for dynamic/extendable filter views
- Chg: New Stream and Stream Filter API
- Enh: Added `topic` content filter concept with stream integration

1.2.8 (July 3, 2018)
--------------------

- Enh: Added user email to javascript user config
- Fix: Module Assets are not republished after module update
- Enh: Added `humhub\components\ModuleManager::EVENT_BEFORE_MODULE_ENABLE` and `humhub\components\ModuleManager::EVENT_AFTER_MODULE_ENABLE` events
- Enh: Added `humhub\components\ModuleManager::EVENT_BEFORE_MODULE_DISABLE` and `humhub\components\ModuleManager::EVENT_AFTER_MODULE_DISABLE` events
- Fix: Improved ZendLucence driver error handling
- Fix #3148: Upload space picture dose not use file size setting in HumHub (acs-ferreira)
- Fix: Incorrect last visit date shown in space admin pending members view (acs-ferreira)
- Enh: Allow enable/disable modules by CLI
- Enh: Added UTC only timezone in server timezone dropdown
- Fix #3176: Integrity checker removes modules default state
- Enh: Updated translations

1.2.7 (May 23, 2018)
--------------------

- Fixed empty modal dialog response issue
- Fix #3146 invalid bootstrap.min.css link in installer
- Enh: Load `humhub\modules\content\models\ContentTagAddition` model in `humhub\modules\content\models\ContentTag::load()`
- Enh: Auto save `humhub\modules\content\models\ContentTagAddition` within `humhub\modules\content\models\ContentTag::afterSave()`
- Enh: Added `humhub\modules\content\components\ContentActiveRecord::isOwner()` to check the ownership of a content
- Enh: Make directory access configurable by `humhub\modules\directory\Module::active`, `humhub\modules\directory\Module::guestAccess`
- Enh: Added `humhub\modules\directory\permissions\AccessDirectory` permission for group level directory access
- Fixed `User `namespace issue in `humhub\modules\user\components\BaseAccountController`
- Chg: Added footer menu to account menu on small display resolutions

1.2.6  (May 14, 2018)
-----------------------

When you are using a custom theme, you may need to add the newly introduced footer navigation to your overwritten view files. You can find a full list of the view changes here: https://github.com/humhub/humhub/commit/a1815fb61d83619ce9ca40166800b8c5dcb9d539

- Fix #3108: Fixed cronjob examples with leading zero (acs-ferreira)
- Fix: Memory leak in activity mail summary processor cron
- Fix: With enabled guest mode BaseAccountController does not redirect to login page
- Enh: Added footer navigation - FooterMenu widget
- Enh: Added HForm class events EVENT_AFTER_INIT and EVENT_BEFORE_RENDER
- Enh: Updated translations

1.2.5  (April 11, 2018)
-----------------------

When you customized or used the createCVS method of PendingRegistrationsController please migrate your code to SpreadsheetExport. PHPOffice is replaced by PHPSpreadsheet.

- Enh: Added BaseURL setting protocol scheme validation
- Fix #2849: ActiveQueryContent doesn't find public profile content when guest access is enabled
- Enh: Fixed username alignment in comments (@githubjeka)
- Enh: More readable WallEntryAddon links (@githubjeka)
- Fix: Documentation grammar fixes (@Felli)
- Fix: Let's Encrypt ACME Error (@Felli)
- Fix: Typo in password recovery (@acs-ferreira)
- Fix: Profile posts of friends not appears on dashboard
- Fix #2745: Yii2 2.0.13 will break the admin interface
- Enh: Allow auto detection of response dataType
- Fix #2947: Allow json success result on modalSubmit
- Enh: Disabled automatic content following on likes by default
- Enh: Improved IntegrityChecker memory usage
- Chg: `PendingRegistrationsController->createCVS` removed
- Fix: Stream image preview size not changeable
- Fix: Increased maximum e-mail address length from 45 characters to 254
- Fix: Group member search by firstname/lastname
- Enh: Added Slovene language
- Enh: Added Croatian language
- Fix: User approval, lastname field is shown twice to admins
- Fix: User model namespace issue in `humhub/modules/user/components/UrlRule`
- Enh: Raised notification over view pagination size to 20
- Enh: Added `humhub/modules/space/models/Module::flushCache()` and `humhub/modules/space/behaviours/SpaceModelModules::flushCache()` in order to flush the space module cache
- Enh: Added further `FunctionalTester` utilities
- Enh: Added Norwegian Nynorsk language
- Fix #3009: Change the Space URL raises 404

1.2.4  (December 13, 2017)
--------------------------

- Enh: Translation updates
- Fix: Added `ManageSpaces` and SystemAdmin check to `UserGroupAccessValidator`.
- Fix: Only include content with `stream_channel = default` into spacechooser update count.
- Enh: Add LinkedIn auth to login. (Felli)
- Enh: Add Twitter auth to login. (Felli)
- Enh: Add Instagram auth to login. (Felli)
- Enh: Add Twitter, LinkedIn & Instagram auth to docs (Felli)
- Enh: Make lucene search term limit configurable via `ZendLuceneSearch::$searchItemLimit`.
- Fix: Empty stream message between friends
- Enh: Improve composer-asset-plugin config (cebe)
- Enh: Added a link to the permalink from the ago text (benklop)
- Enh: Added directory group description (githubjeka)
- Enh: Added configuration option to include user profile posts in dashboard without following
- Fix: User profile sidebar disappered
- Fix: Like notification for comments not working
- Fix: Add example users to default Users group
- Fix #2851: getting model attribute value using Html::getAttributeValue()
- Fix #2844: Directory member search broken on page 2
- Fix #2702: Disable content search for guest users due to space visibility
- Fix #2806: Register process broken on some environments (Felli)

1.2.3  (October 23, 2017)
-------------------------

Important note for LDAP users: There is a new setting "ID Attribute" which should be set to clearly identify users. Important note for Git/Composer installations: http://www.yiiframework.com/news/148/important-note-about-bower-and-the-asset-plugin/

- Fix: Readonly markdown field issue.
- Enh: Fixed registration approval/denial mails and made their default value configurable.
- Enh: Updated primary auth client interface for more flexibility
- Enh: Added LDAP ID attribute to improve user mapping
- Enh: Option to disable e-mail address requirement in User model
- Fix: Overwrite of static image in theme + added documentation section
- Fix: Account Controller exception when user is not logged in
- Fix: Exception on notification overview page when not logged in
- Enh: Added possibility to sort groups in directory
- Enh: Removed LDAP UserFilter/LoginFilter length restriction
- Fix: UTC timezone issue with `TimeZoneDropdownAddition` and added `$includeUTC` flag to `TimezoneHelper::generateList()`
- Fix: ControllerAccess json rule
- Enh: added `closable = false` as default `ModalDialog` widget setting
- Fix: trigger richtext `clear` when submitting comment.
- Fix: missing return in `FileContent::beforeValidate`
- Fix: Mentioning search with `-` not working
- Fix #2730: Mentioning search with `-` not working
- Fix: File search with suffix not working
- Enh: Added SearchAttributesEvent to improve content addon indexing (comment/file)
- Fix: Do not automatically force modal close on stream edit
- Enh: Added DurationPickerWidget
- Enh: Allow `ContentActiveRecord($contentContainer, $config)` initialization
- Fix: `WallEntry::addControl` with simple array options
- Enh: Added `$scheme` Argument to `DownloadFileHandler::getUrl()`
- Fix: Clear UserModule cache after save/delete
- Fix: Prevent Integrity check failures.
- Enh: Added default open content as modal action
- Enh: Added possibility to add attachments in Notification MailTarget
- Enh: Added surpressSendToOriginator Notification option
- Chg: #2745 Removed `GroupPermission::instance()` for yii 2.0.13 compatibility
- Enh: Added `MobileTargetProvider` abstraction for mobile push notifications
- Enh: Added `humhub:notification:updateCount` js event
- Enh: Show space administrators and moderators in member snippet
- Fix: `humhub\modules\live\Module::getLegitimateContentContainerIds` behaviour with friendship module enabled
- Enh: Added `BaseNotification:priority` to mark high priority notifications
- Enh: Added new `User::isVisible` and `ActiveQueryUser::visible` methods
- Fix: MarkdownEditor cursor position after inserting file/
- Fix: Make sure own profile content is always visible to user
- Fix #2501: Do not try to embed Youtube unauthorized videos (acs-ferreira)
- Fix #2613: Wrong username encoding with pretty url (githubjeka)
- Fix #2791, #2749: Force private join policy on private spaces + non changeable post visibility
- Fix wrong Comment date issue in notification mails
- Enh: Added `data-file-*` attributes to download links, for beeing able to intercept file downloads
- Enh: Added `apple-mobile-web-app-*` and `mobile-web-app-capable` meta tags to `head.php`
- Fix #2783: E-Mail notification link broken when guest mode is enabled (Buliwyfa)
- Enh: Added `ContentActiveRecord::silentContentCreation` for disabling ContentCreated Activity/Notification on ContentActiveRecord level
- Enh: Now the `NewContent` live event is always fired with `sourceClass` and `sourceId` information and a `silent` flag for silent content creations

1.2.2  (August 2, 2017)
--------------------------------
- Enh: Allow returning class names beside BasePermission instances in `Module::getPermissions()`
- Enh: Increase profile image size to 800px.
- Fix #2644 overlapping popup preview image after increasing preview image size (hagalaz)
- Fix: Button widget child class static instantiation not working
- Fix: ModalButton instantiation and added ModalButton::close()
- Fix: Respect `max_file_uploads` setting in UploadInput widget
- Enh: Include `kartik-v/yii2-widgets`
- Enh: Added `getAccessRules()` to `humhub/components/Controller`
- Fix: AccessControl action restriction bug
- Fix: `ModuleAutoLoader` exceptions not logged
- Fix: `I18N` formatter user timezone not set
- Enh: Automatically set space default visibility in `Content::setContainer()`
- Fix: Fixed ContentContainerSettingManager caching issue if space/user id are equal
- Enh: Use of select2 dropdown for time zone selections
- Fix: Bypass AccessControl behavior in installer
- Fix: Use of JS-Widget internal event object instead of node
- Enh: Added `Formatter::getDateTimePattern()` and `Formatter::isShowMeridiem()`
- Fix: Set formatter locale in I18N when changing locale
- Enh: Added `$hideInStream` flag for upload component/action for changing `show_in_stream` file flag
- Enh: Added `$showInStream` flag for `FilePreview` widget to only include files with certain `show_in_stream` flag
- Enh: Added `FileManager::findStreamFiles()` for querying files with either given `show_in_stream = 1` or `show_in_stream = 0` flag.
- Enh: Added `humhub\widgets\Tabs` and `humhub\widgets\SettingsTabs` with view type tab support
- Enh: Added new `MarkdownField` input widget which as replacement of deprecated `MarkdownEditor`
- Fix: Fixed markdown file upload pjax issue
- Fix: Removed `display: table-cell` from markdown image css to enable inline images
- Enh: Added `humhub/widgts/Button::userPickerSelfSelect()` for creating self select button for userpickers.
- Enh: Added `humhub/widgts/Link::withAction()` for creating action based links
- Enh: Added `SelectTimeZoneDropdown` widget
- Enh: Added `Modal::closable` in order to respect `backdrop` and `keyboard` data setting of `Modal` and `ModalDialog` widget
- Enh: Avoid cutting oembed entry in stream if it's the first part of a richtext
- Enh: Added `humhub/widgets/TimePicker` widget
- Enh: Added `DbDateValidator::timeZone` for setting input time zone
- Enh: Additional WallEntry settings: `$jsWidget`, `$addonOptions`, `$controlsOptions`, `$renderControls`, `$renderAddons`
- Enh: Added possibility to overwrite WallEntry settings in `humhub/stream/actions/Stream::renderEntry()`
- Enh: Added `ShowFiles::preview` and `ShowFiles::active` flag
- Enh: Allow `$adminOnly` for User base ContentContainerController Controller
- Enh: Added `ContentContainerActiveRecord::getDefaultContentVisibility()` and `User::getDefaultContentVisibility()`
- Enh: Added automatic Notification Class loading by convention. No need to overwrite `Module::getNotifications()`
- Enh: Added `ContentActiveRecord::getIcon()` for adding an badge icon to WallEntry content type badge
- Enh: Added `ContentActiveRecord::getLabels()` for managing WallEntry labels (badges)
- Enh: Added `Label` widget for creating sortable labels
- Fix: Reset modal dialog size + add `size` option
- Enh: Added `size` option `ui.modal.Modal.set()`
- Enh: Use `ContentActiveRecord::getUrl()` for content perma links (if given)
- Enh: Added `ContentTag` concept for creating content categories/filter on module level
- Fix: Mentioning keeps running even if previous input result was empty
- Enh: Darkened comment links for better readability
- Fix #2582 Userfollow activity click action not working
- Enh: Make space membership activities clickable
- Chg: Removed `yii2-codeception` dependency
- Chg: Added `phpoffice/phpexcel` dependency
- Enh: Added `JsWidget::fadeIn` for smooth widget initialization
- Enh: Enhanced `AccessControl` filter with `ControllerAccess` layer for better testability and flexibility
- Enh: Added `Pending Registrations` admin view with `csv`, `xlsx` support.

1.2.1 (June 17, 2017)
--------------------------------
- Fix: Invite error in french language
- Fix #2518: ActivityStreamWidget::EVENT_INIT is missed (githubjeka)
- Enh: Fixed accessibility issues in Dashboard/Login/Profile
- Fix: module beforeInit and afterInit event
- Enh: Added Registraion::EVENT_AFTER_REGISTRATION UserEvent
- Enh: Added grunt `migrate-up` and `migrate-create` task
- Enh: Added profile field type `CheckboxList`
- Fix: Fixed `ui.addition` `MutationObserver`, only apply additions to inserted nodes.
- Enh: Changed invite mail subject text
- Fix #2571: last_login not set after registration direct login
- Enh: Always trigger dom widget events for widget `fire` until `triggerDom` is set to false
- Enh: Added `richtextPaste` event
- Enh: On search index rebuilding - use batch queries
- Fix: `ActiveQueryContent:readable()` for guNest users missing join
- Enh: Added `ContentActiveRecord:managePermission` for changing the default write permission of ContentActiveRecord classes
- Enh: Moved all default `WallEntryControls` to `WallEntry:getContextMenu()` widget.
- Fix: Connect google OAuth under `Profile Settings -> Connected Accounts` throws invalid redirect uri.
- Fix: Invite Users does not respect ManageUsers/ManageGroups permission
- Fix: Mail summaries sent in incorrect language
- Fix: Send button text on request space membership dialog
- Fix #2555: Friendship notification category visible even if friendship system deactivated
- Enh: Don't auto focus space chooser search on small devices
- Fix #2612: Single list item hides markers
- Fix #2558: No notification for user profile posts send
- Fixed #2560: Markdown profile field editable flag not working
- Fix: Hide also header (space, profile) counts when following system is disabled
- Fix: Perma link to space contents broken when space homepage was changed
- Fix: Properly sort language and country select by users locale
- Enh: Allow search in country profile field dropdown
- Fix: js action api empty data attribute
- Enh: Added button helper widgets `<?= Button::primary('myButton')->action('myJsAction')?>`
- Enh: Enhanced ContentActiveRecord instantiation `$model = new MyContent($space, Content::VISIBILITY_PRIVATE)`
- Fix #2625 Pjax problem with local links to files within stream
- Enh: Use of `target="_blank"` for stream links
- Fix #2594 Bug: Url with unicode in stream markdown
- Fix: Notification grouping not working
- Fix: Show more suppression entries with sort order update + equal update_at not working.
- Fix #2627: Incorrect language used in group admin user approval e-mail
- Fix #2631: Module configuration link shown for disabled modules
- Fix #2785 #2172: Added iconv PHP extension to the requirement check (leuprechtroman)

1.2.0 (April 16, 2017)
--------------------------------
- Fix: SVG file uploads broken (mime type: image/svg+xml)
- Fix: Public badge missing after create post
- Fix: Mentioning notificaiton in user not working
- Fix: Catch yii\db\Expression error for updated_at in wallentry
- Enh: Added 'client.back' js action
- Fix #2219: Overlapping summary mail content
- Fix: Wall entry layout link/text overflow
- Fix: Stream - Do not surpress if only particual contents are displayed
- Fix: GlobalModal extends base Modal widget and GlobalModal::$backdrop is false by default (githubjeka)
- Fix: Search StreamEntry options delete/editModal
- Fix: Tour popover close behaviour
- Fix: Incorrect permissions in space with guest mode

1.2.0-beta.4 (March 28, 2017)
--------------------------------
- Fix: Notification count '0' visible after click on notification link
- Fix: Default space permissions not adopted
- Fix: Use of $permission->getId() instead of $permission->id in PermissionManager (allow dynamic permission ids)
- Fix #2393: Markdown h4,h5,h6 broken
- Fix #2389: calculate max upload file size on PHP 7.1 (githubjeka)
- Fix: LDAP - Lost authclient ldap class configuration on user update
- Fix #2400: Space ownership transfer form shows wrong users
- Fix: Enable user approval without available registration groups or default group
- Fix: Activate 'User' navigation in Admin Menu "Administration -> User -> Settings"
- Enh: Improved administration user deletion view
- Enh: Added 'containerLink' HTML Helper method
- Enh: WallEntry layout layout improvements
- Fix: Default user & space module configuration lost after foreign key migration
- Fix: Respect pinned post when inserting a a new stream entry
- Fix: Show comments in modal not working
- Fix: #2374 Comment input not focused on comment link click
- Enh: Toggle comment box
- Enh: Added global copyToClipboard
- Enh: Added "weekly" mail summary interval
- Fix: Invalid temp.css file
- Fix: Default stream sort setting not applied
- Enh: Show different login message, when registration is disabled
- Fix: Norwegian translation code for Yii messages
- Fix: Also allow comment editing by admins if content 'adminCanEditAllContent' is enabled
- Enh: Added Make Private/ Make Public link to wall entry controls
- Enh #2392: Added Latvian language
- Fix: Hide image file info setting
- Fix #2297: Failed to open stream: No such file or directory when attaching files in UploadAction

1.2.0-beta.3 (March 20, 2017)
--------------------------------
- Enh: Added Grunt tasks `build-assets`, `build-theme`, `build-search`
- Fix: Error when saving account setting permission.
- Fix: #2296 stream scroll issue for mobile webkit browsers (martinbeek)
- Fix: Added unknown upload error if server cancels upload (e.g in case of a post_max_size violation issue)
- Enh: Added warning if php max upload/post is less than the humhub setting.
- Enh: Added mp4/ogg blueimp support in post gallery
- Enh: Added global (default) notification space settings
- Enh: #2359 Use Jplayer playlist feature for post mp3
- Enh: added js module 'ui.view' for view state and utils - Changed 'ui.state.getState' to 'ui.view.getState'
- Enh: added view helper as getHeight/Width and isSmall/Medium/Normal (width) to 'ui.view' js module
- Fix: removed popover image preview from mobile
- Fix: removed target-densitydpi not supported warning
- Enh: Added Stream::renderEntry for rendering Streamentries from ContentActiveRecord
- Fix: Wallentry menu not working in search view
- Fix: Double notifications when mentioning in comments
- Enh: Raised collapse value for posts to full embeded youtube video height
- Fix: Fixed oembed post edit
- Enh: Included select2-humhub theme into the new theming
- Enh: Added select2 dropdown for language selection in account and admin settings
- Enh: Added data-ui-select2 addition for simple select2 dropdowns
- Fix: Don't apply js additions if there was no matching element
- Fix: #2336 use of invalid message key in comment notification (dutch)
- Enh: Disable user and space follow by means of module settings
- Fix: Setting of submitName and upload input name in file upload JsWidget
- Fix: Rendering of UploadButton without given id
- Enh: Added preventPopover and popoverPosition options to file preview
- Enh: Added uploadSingle option for uploads with only one file
- Fix: Missing margin of wall-entry-controls in comments
- Enh: Added alignHeight setting to js loader module
- Enh: Allow Response as arguments for modal.setDialog
- Enh: Enable modal loading events with dataType json
- Enh: Allow direct class export instead of module export in JS Modules e.g. module.export = MyClass
- Enh: Added xhr to client response instances
- Enh: Added response.header for receiving response header from xhr
- Enh: Added post action to client module for data-action-click="client.post"
- Fix: Try using options url as fallback in client calls if the action instance does not provide an url. e.g. client.post(evt, {url:...}
- Enh: Enable setting ajax dataType from trigger e.g. data-action-click="modal.load" data-action-data-type="json"
- Enh: Added action event.data for receiving action specific data options
- Enh: Added default run for JsWidget
- Enh: Added File::findByRecord for searching all attached files of a given ActiveRecord
- Fix: Only set js view state for non full page load and pjax
- Fix: Small gap on TopNav mouse hover (acs-ferreira)
- Enh: Humand readable file sizes. (acs-ferreira)
- Enh: Changed default $minInput of SpacePickerField to 2. (githubjeka)
- Fix: Error when saving "Administration -> Settings -> General" without default space. (githubjeka)
- Fix: #826: Notification status not updated right after like.
- Fix: #2316: Reinvitation by email not working
- Fix: #2314: Html helper namespace issue in Markdown.php class
- Fix: #2302: Hide file info for images on wall settings not applied.
- Fix: German translation error in Admin -> Users -> Groups -> Members -> Add Member UserPicker.
- Fix: German translation "Notify Users" placeholder too long.
- Fix: Admin group add members placeholder.
- Fix: Stream entry root not removed for content delte (poll,etc)
- Enh: Easier save feedback by using 'module.log.success('saved')'
- Fix: Admin group add members placeholder.
- Enh: Easier save feedback by using module.log.success('saved');
- Fix: Set jsWidget id when autogenerated
- Fix: Use of Html::activeLabel instead of $form->label in RichtextField
- Enh: Added pjax redirect capability to js client
- Fix: Show default error in status bar if invalid message object was provided
- Fix #2304: Users not loaded in user selection fields.
- Enh: Added User module 'displayNameCallback' attribute for custom display name formats
- Enh: Added Clipboard.js and Permalink "Copy to clipboard" link
- Enh: Validate minimum PHP version in Console Application
- Enh: Added optional ActiveRecordContent::canEdit() method for custom ACLs
- Fix: Better error handling/logging on corrupt GD Image files
- Fix #2288: Pjax breaks OAuth2 ReturnUrl
- Fix: Incorrect First name & Last name message key (githubjeka)
- Fix: Do not store complete comments with search index (helnokaly)
- Fix #2319: Run console application before installation
- Fix: Directory Knob statistics on included modules (e.g. Enterprise Edition)
- Enh: Added widget to display user profile image
- Enh: Directory view templates cleanups
- Fix: All LDAP Users have been disabled and not reenabled by hourly cronjob if ldap server not reachable.
- Enh: Cleanup authentication layout file
- Fix: Console image converter memory limit allocation
- Enh: Added new controller init event
- Enh: Made admin base controller method "getAccessRules()" non static
- Enh: Created new ImageController for user image and banner handling
- Enh: Decreased OEmbed url max length 180chars (acs-ferreira)
- Enh: Added APCu Support
- Enh: Added ContentContainer integrity check (Daha62)
- Fix #2331: Bug image load on PHP 7.1 with dynamic memory alloc (githubjeka)
- Fix #2367: `ImageConverter::allocateMemory` uses common units(MegaBates) of memory (githubjeka)
- Fix: #2369: typo issue (Felli)
- Fix: Better notification compatiblity - mail views and enabled WebNotificationTarget
- Fix #2312: Pinned post appears twice on stream
- Enh: Added option to show/hide deactivated user content in stream
- Enh: Allow any url route as homepage by homeUrl array application parameter
- Fix #2255: Added missing Social Account Settings menu
- Fix: Added missing file download http caching
- Enh: Added console email test command
- Enh: Added stream module defaultStreamSuppressQueryIgnore to ease overwrites
- Enh: Added 'archived' badge to archived spaces in directory

1.2.0-beta.2 (February 24, 2017)
--------------------------------
- Fix: TimeAgo locale not loaded in production mode, added AppDynamicAsset (luke-)
- Enh: Translation message rebuild and auto translated duplicates (luke-)
- Enh: Combined all directory translations into base message category (luke-)
- Enh: Added logging table cleanup job (luke-)
- Enh: Added new version check as ActiveJob (luke-)
- Enh: Moved user configuration params 'minUsernameLength' + 'adminCanChangeProfileImages' to user module class (luke-)
- Enh: Added .editorconfig code style configuration file (luke-)
- Enh: Added 'show_in_stream' column in file table to hide output in wall entries (luke-)
- Enh: Added 'renderGalleryLink' link method to PreviewImage converter (luke-)
- Fix: Search view links not working (buddh4)
- Fix: Markdown in comment layout issue (buddh4)
- Enh: humhub.ui.showMore module for cutting post text and comments (buddh4)
- Fix: Javascript issues with guest users, removed initialitation of some modules for guest user (buddh4)
- Fix: Mutliple use of same emoji in richtext.
- Enh: Use of Yiis new afterRun for humhub Widgets.
- Fix: Word break issue in markdown posts.
- Fix: Richtext with emoji only on post edit where ignored.
- Enh: Added data-action-confirm for confirming actions.
- Fix: File StorageManager setContent method broken
- Enh: Added FileHelper methods createLink & getContentContainer
- Enh: Javascript HumHub Client - better handle ajax redirects
- Enh: TopMenu / TopMenuRightStack hide content when user is not logged in without guest mode
- Enh: Added showUserName option in AccountTopMenu widget
- Enh: Added isGuestAccessEnabled method in User component
- Enh: Added flash variable (executeJavascript)to execute js on the next page load
- Enh: Added possibility to create own file handlers (edit, create, import, export)
- Enh: Added data-action-process to handle modal processes
- Enh: Added upload file event (humhub:file:created)
- Enh: Added custom file handler positions
- Enh: Moved UploadAction::getFileResponse method to FileHelper::getFileInfos
- Enh: Added JS context menu to ui.additions module
- Enh: Enhanced ContentContainer Module enable/disable
- Enh: Added client.reload for pjax and non pjax page reloads
- Enh: Added ContentContainerAsset to AppAsset
- Enh: Added editModal for editing wallentries within a modal instead of inline
- Fix: Oembed not rendered in richtext.
- Enh: Smarter show more logic - Only cut text if it overlaps the max height by a specific span.
- Enh: Added getContextMenu for defining wallentry context options.
- Enh: Added editMode to WallEntry for allowing modal based edits.
- Fix: file-preview text overflow in HumHub theme.
- Fix #2280: Meta data (rotation) not respected for camera images (ImageMagick)
- Fix: Activity stream rendering issue on page unload.
- Enh: Optimized stream entry fade animation.
- Enh: Added $maxAttachedFiles to content module to restrict the uploaded file count of comments and posts
- Fix: Hide notification count badge if notification count is 0
- Fix: Only flush js config if not empty
- Enh: Use of theme variables in mail all views
- Fix: Submit comment with only files leads to Internal Server Error
- Fix: Prevent spacechooser message count update on own content creation
- Fix: Abort overlapping space chooser search requests
- Fix: Problem in notification group_count with only one involved user
- Fix #2257: Set module as default in space/user broken

1.2.0-beta.1 (February 08, 2017)
--------------------------------
- Enh: Moved HumHub browser icons to HumHub theme (luke-)
- Enh: Moved support css/js for older IE version into own AssetBundles (luke-)
- Enh: Moved CSRF Tag output to View renderHeader (luke-)
- Enh: Moved LayoutAddons widget from main layout to View endBody() method (luke-)
- Enh: Added PJax page loading (luke-)
- Enh: Refactored File module (luke-)
- Enh: Added yii2-imagine Extension (luke-)
- Enh: Use of blueimp image gallery (buddha)
- Enh: JS module system with build in logging/text/config features (buddha)
- Enh: JS core api under humhub namespace (buddha)
- Enh: Use of compressed assets (js,css) in production mode (buddha)
- Enh: Enhanced testability (buddha)
- Enh: Added administrative backend group permissions (buddha)
- Enh: Enhanced AccessControl filter with permission rules. (buddha)
- Enh: Splitted less files to facilitate theming. (buddha)
- Enh: Added user status bar for user feedback (buddha)
- Enh: Better UserFeedack (buttons/messages) / Replacement of old DataSaved widget (buddha)
- Enh: Overwrite default permission settings (buddha)
- Enh: SpaceChooser rewrite with following spaces and remote search (buddha)
- Enh: Modal widget rewrite.
- Enh: Enhanced Archived Space handling (buddha)
- Enh: Upload widget rewrite. (buddha)
- Enh: Picker widgets rewrite (UserPicker/SpacePicker/MultiselectDropdown). (buddha)
- Enh: Richtext widget rewrite. (buddha)
- Enh: Removed almost all inline JS blocks. (buddha)
- Enh: StreamAction now uses flexible StreamQuery Model. (buddha)
- Enh: Post markdown support. (buddha)
- Enh: Added 'live' module for push/pull messages to the frontend (luke-)
- Enh: Added asynchronous job queues (luke-)
- Enh: Changed minimum PHP version to 5.6
- Enh: Added possibility of global content (content w/o contentcontainer) (luke)
- Enh: Added new profile field type: checkbox (luke-)
- Enh: Refactored mail summaries activity module (luke-)
- Enh: Moved all static files (js, fonts, css) into own static folder @web-static (luke-)
