2. Sections
===============
Backend (Called waavadmin) and Frontend (called controlroom or clipbucket)


#. Waavadmin (https://dev5.waav.com/waavadmin || /waavadmin)
    * Laravel (Older 5.1 version running on PHP 5.6 || Both outdated, we already have a task to work on todo list for upgrade) - PHP8 & Laravel 11

#. ControlRoom (https://dev5.waav.com/trains || /trains)
    * Trains is actually a company. This company is used as a template. When deploying changes to production, we copy the trains and overwrite the company directory
    * Each company has given a subdomain and has its own file directory (This we want to work on to use single common template). This got ended up like this because of use of a one of old (Not much popular PHP framework) - clipbucket - https://clipbucket.com/ (We want to change to Laravel in future)

#. Portal (https://dev5.waav.com/trains/portal)
    * Own npm system for JS package management
