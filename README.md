<a href="https://www.htmly.com" target="_blank">![Logo](https://raw.githubusercontent.com/danpros/htmly/master/system/resources/images/logo-big.png)</a>

[HTMLy](https://github.com/danpros/htmly) is an open source databaseless web publishing platform written in PHP.

This quickstart will creating installer.php and setup the environment inside `$OPENSHIFT_DATA_DIR` and `$OPENSHIFT_REPO_DIR`. To install HTMLy simply visiting `yourapp.rhcloud.com/installer.php` after deploying it using the console and than create your blog username and password there.

HTMLy have a cloud update feature and fetch the sources from Github repo, so no need to update the app using git but simply visiting the HTMLy update page and if a newer version available you just need to follow the update link.

If you need to add or modify the theme or creating new user you must use FTP instead of git. All files are saved inside `$OPENSHIFT_DATA_DIR/www` and the `$OPENSHIFT_REPO_DIR` is just a placeholder that contains the `www` symlink to HTMLy installation directory.

**Quick install:**

[![Click to install OpenShift](http://launch-shifter.rhcloud.com/launch/light/Click to install.svg)](https://openshift.redhat.com/app/console/application_type/custom?&cartridges[]=php-5.4&initial_git_url=https://github.com/danpros/htmly-openshift.git&name=htmly)

**Step by step:**

* Create your application using the console.

* For cartridge you can choose PHP 5.3, PHP 5.4 (recommended), or PHP 5.4 with Zend Server 6.1.

* Set your public URL, and for source code put `https://github.com/danpros/htmly-openshift.git`. Click `Create Application`.

* Visit `yourapp.rhcloud.com/installer.php` to start the installation.

**Demo blog:**

[HTMLy OpenShift Demo](http://www.directorize.com)
