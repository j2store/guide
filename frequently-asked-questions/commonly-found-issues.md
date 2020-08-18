# Commonly found issues

## On update to 3.3.6 <a id="on-update-to-336"></a>

Starting from the release 3.3.6, when you install the latest version of J2Store on your site over an existing version, you might find a warning that looks like this:

 

![PHP error](https://raw.githubusercontent.com/j2store/doc-images/master/frequently-asked-questions/commonly-found-issues/error-j2store-exists.png)

**Why it occurs?**

This is just a warning. This warning indicates that there is already an existing version of J2Store available on the site and now a new version has been installed over an existing version.

**Will this harm my site?**

No, this warning wouldn’t affect the site in any way. As mentioned before, this is just a warning and you could ignore this.

## Due to the backward compatibility to earlier versions of PHP <a id="due-to-the-backward-compatibility-to-earlier-versions-of-php"></a>

Sometimes, you could find a warning like this on your site:  

![PHP backward compatibility](https://raw.githubusercontent.com/j2store/doc-images/master/frequently-asked-questions/commonly-found-issues/warning-php.png)

**Why it occurs?**

This warning occurs when you turn on Error reporting on your site’s global configuration under System-&gt;Global configuration-&gt;Server tab.

This occurs since we provide backward compatibility to the earlier versions of PHP.

**Will this harm my site?**

No, this wouldn’t harm your site in anyway. To overcome this, you could turn off the error reporting under Joomla global configuration.\*\*

**Why it occurs?**

This warning occurs when you turn on Error reporting on your site’s global configuration under System-&gt;Global configuration-&gt;Server tab.

This occurs since we provide backward compatibility to the earlier versions of PHP.

**Will this harm my site?**

No, this wouldn’t harm your site in anyway. To overcome this, you could turn off the error reporting under Joomla global configuration.\*\*

## Issue: <a id="issue"></a>

**Unable to save anything on the site**

This might be because of two prominent reasons.

* **Database type**

The **database type** should be set to **MySQLi** \(the one that is supported by J2Store\) under System-&gt;Global configuration-&gt;Server tab. 

![Database-type](https://raw.githubusercontent.com/j2store/doc-images/master/frequently-asked-questions/commonly-found-issues/database-type.png)

* **Caching**

This issue might also be because of caching. Try clearing cache and disabling the site, browser and server-side caching if any and then try saving the settings.

