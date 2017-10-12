---
TOCTitle: Update storage issues
Title: Update storage issues
ms:assetid: 'f7c31b39-b056-4ee5-9966-cd63b2ad16d8'
ms:contentKeyID: 18155375
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708624(v=WS.10)'
---

Update storage issues
=====================

Updates can be stored on the local WSUS server or on Microsoft Update. Use this section to troubleshoot problems with update storage.

The updates listed in the WSUS console do not match the updates listed in your local folder
-------------------------------------------------------------------------------------------

This can happen under different circumstances. For example, if updates are stored on a disk separate from the WSUS application itself, and that disk fails, when you replace the failed disk with a new (empty) disk, the WSUS application will still show all of the updates as downloaded.

To have WSUS verify which updates are stored on the disk, you must run the WSUSutil.exe using the **reset** command.

| ![](images/Cc708624.note(WS.10).gif)Not                 |
|--------------------------------------------------------------------------------------|
| Performing a reset causes the WSUS server to be unresponsive for up to five minutes. |

**To have WSUS verify locally stored updates**
1.  Click **Start**, and then click **Run.**

2.  In the **Open** box, type **cmd**, and then click **OK**.

3.  At the command prompt, navigate to the directory that contains WSUSutil.exe.

4.  Type the following, and then press ENTER: **wsusutil.exe reset**
