# File and server settings

Set sensible file permissions, disable editing that is not needed, and protect sensitive files so that even if an attacker gets a foothold, the damage they can do is limited. These settings will not stop an attack on their own, but they reduce what a successful one can reach.

## File permissions

File permissions control who can read and change files on the server. Permissions that are too open let a compromised process modify files it should not. The general principle is least privilege: files and directories should be writable only where WordPress genuinely needs to write, and no more. Your host's documentation usually gives recommended values; the point is that wide-open permissions are a risk worth closing.

## Disable the built-in file editor

WordPress includes an editor that lets administrators change theme and plugin code from the dashboard. If an administrator account is compromised, that editor becomes a direct way to inject malicious code into the site. Disabling it removes that path, so an attacker who gets into the dashboard cannot edit site files through it. For most sites, the editor is a convenience that is not worth the risk.

## Protect the configuration file

The main configuration file holds database credentials and secret keys, so it is one of the most sensitive files on the site. Ensure it is not readable from the web and that its permissions are tight. Exposure of this file hands an attacker the keys to your database, so protecting it is a high priority among file-level measures.

## Limit what runs in upload directories

Directories where users or the site can upload files should not be allowed to execute code. An attacker who manages to place a file in an uploads folder should not be able to run it. Configuring the server so that upload directories serve files but do not execute them closes a common path from an upload to a running exploit.

## Hide what does not need to be public

Reduce the information your site volunteers about itself, such as detailed version numbers and error messages that reveal internal paths. This is not a strong protection by itself, but giving attackers less to work with is a reasonable default. The aim across all of these settings is the same: assume something might get through, and limit how far it can go.
