---
TOCTitle: 'Appendix I: Database Maintenance'
Title: 'Appendix I: Database Maintenance'
ms:assetid: 'e787794b-4f09-4d01-ae4e-5983ea7634f9'
ms:contentKeyID: 18155326
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708594(v=WS.10)'
---

Appendix I: Database Maintenance
================================

In order to keep your WSUS server functioning correctly, you should have a maintenance plan that includes re-indexing the database on a regular basis, preferably at least once a month.

The [WsusDBMaintenance](http://go.microsoft.com/fwlink/?linkid=87027) script (http://go.microsoft.com/fwlink/?LinkId=87027) allows you to re-index any version of the SUSDB database, either SQL Server 2005 or Windows İç Veritabanı.

If you are using Windows İç Veritabanı, you will need to use the **sqlcmd** utility, which can be downloaded from [Feature Pack for Microsoft SQL Server 2005](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728). For more information about the **sqlcmd** utility, see [sqlcmd Utility](http://go.microsoft.com/fwlink/?linkid=81183) (http://go.microsoft.com/fwlink/?LinkId=81183).

        ```
where *&lt;scriptLocation&gt;* is the directory where you have copied the WsusDBMaintenance script.
