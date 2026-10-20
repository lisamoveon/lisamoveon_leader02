Working with Remote Documents
===================================

Oxygen XML Editor supports editing remote files, using the WebDAV, SharePoint Online for Office 365, or SFTP
protocols. You can edit remote files in the same way you edit local files. For example, you can add remote files
to a project, or use them in XSL and FO transformations.

Server Type
---------------

Specifies the type of server. You can choose between:
• WebDav FTP - For generic HTTP/SFTP/WebDav and other servers.
• SharePoint Online - For SharePoint Online servers.

WebDAV over HTTPS
---------------------

If you want to access a WebDAV repository across a non-secure network, Oxygen XML Editor allows you to
load and save the documents over the HTTPS protocol (if the server understands this protocol) so that any
data exchange with the WebDAV server is encrypted.
When a WebDAV repository is first accessed over HTTPS, the server hosting the repository will present a
security certificate as part of the HTTPS protocol, without any user intervention. Oxygen XML Editor will 
use this certificate to decrypt any data stream received from the server. For the authentication to succeed
you should make sure the security certificate of the server hosting the repository can be read by Oxygen
XML Editor. This means that Oxygen XML Editor can find the certificate in the key store of the Java Runtime
Environment where it runs. You know the server certificate is not in the JRE key store if you get the error No 
trusted certificate found when trying to access the WebDAV repository.