---
title: Arbeiten mit Office 365-Verwendungsberichten in Microsoft Graph
description: Mit Microsoft Graph können Sie auf Office 365-Verwendungsberichtsquellen zugreifen, um Informationen darüber zu erhalten, wie Mitarbeiter in Ihrem Unternehmen Office 365-Diensten nutzen. Sie können zum Beispiel identifizieren, wer einen Dienst häufig verwendet und Kontingente erreicht oder wer vielleicht gar keine Office 365-Lizenz benötigt.
ms.openlocfilehash: 81e0bc649c8475ac6b83a74f3552e83ce0c3ddb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059009"
---
# <a name="working-with-office-365-usage-reports-in-microsoft-graph"></a>Arbeiten mit Office 365-Verwendungsberichten in Microsoft Graph

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Mit Microsoft Graph können Sie auf Office 365-Verwendungsberichtsquellen zugreifen, um Informationen darüber zu erhalten, wie Mitarbeiter in Ihrem Unternehmen Office 365-Diensten nutzen. Sie können zum Beispiel identifizieren, wer einen Dienst häufig verwendet und Kontingente erreicht oder wer vielleicht gar keine Office 365-Lizenz benötigt.

## <a name="authorization"></a>Authorization

Microsoft Graph steuert den Zugriff auf Ressourcen über Berechtigungen. Sie müssen die benötigten Berechtigungen angeben, um auf Berichtsressourcen zugreifen zu können. In der Regel geben Sie Berechtigungen im Portal Azure Active Directory (Azure AD) an. Weitere Informationen finden Sie unter [Microsoft Graph-Berechtigungsreferenz](/graph/permissions-reference) und [Berichtsberechtigungen](/graph/permissions-reference#reports-permissions).

## <a name="changes-to-the-reports-apis"></a>Änderungen an der Reports-APIs

Die ursprünglichen Berichte APIs wurden aktualisiert, damit die API für die bestimmte Ansicht aufgerufen werden kann, die anstelle einen View-Parameter übergeben werden sollen. Es wird empfohlen, dass Sie mit den neuen APIs in Ihrer Anwendung so bald wie möglich zu starten. Die folgende Tabelle enthält die APIs, die entfernt wurden und die neuen APIs, die sie ersetzt.

| Ursprüngliche-API            | Neue API                                  |
| :---------------------- | :--------------------------------------- |
| EmailActivity           | <ul><li>[getEmailActivityUserDetail](../api/reportroot-getemailactivityuserdetail.md)</li><li>[getEmailActivityCounts](../api/reportroot-getemailactivitycounts.md)</li><li>[getEmailActivityUserCounts](../api/reportroot-getemailactivityusercounts.md)</li></ul> |
| EmailAppUsage           | <ul><li>[getEmailAppUsageUserDetail](../api/reportroot-getemailappusageuserdetail.md)</li><li>[getEmailAppUsageAppsUserCounts](../api/reportroot-getemailappusageappsusercounts.md)</li><li>[getEmailAppUsageUserCounts](../api/reportroot-getemailappusageusercounts.md)</li><li>[getEmailAppUsageVersionsUserCounts](../api/reportroot-getemailappusageversionsusercounts.md)</li></ul> |
| MailboxUsage            | <ul><li>[getMailboxUsageDetail](../api/reportroot-getmailboxusagedetail.md)</li><li>[getMailboxUsageMailboxCounts](../api/reportroot-getmailboxusagemailboxcounts.md)</li><li>[getMailboxUsageQuotaStatusMailboxCounts](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md)</li><li>[getMailboxUsageStorage](../api/reportroot-getmailboxusagestorage.md)</li></ul> |
| Office365Activations    | <ul><li>[getOffice365ActivationsUserDetail](../api/reportroot-getoffice365activationsuserdetail.md)</li><li>[getOffice365ActivationCounts](../api/reportroot-getoffice365activationcounts.md)</li><li>[getOffice365ActivationsUserCounts](../api/reportroot-getoffice365activationsusercounts.md)</li></ul> |
| Office365ActiveUser     | <ul><li>[getOffice365ActiveUserDetail](../api/reportroot-getoffice365activeuserdetail.md)</li><li>[getOffice365ActiveUserCounts](../api/reportroot-getoffice365activeusercounts.md)</li><li>[getOffice365ServicesUserCounts](../api/reportroot-getoffice365servicesusercounts.md)</li></ul> |
| Office365GroupsActivity | <ul><li>[getOffice365GroupsActivityDetail](../api/reportroot-getoffice365groupsactivitydetail.md)</li><li>[getOffice365GroupsActivityCounts](../api/reportroot-getoffice365groupsactivitycounts.md)</li><li>[getOffice365GroupsActivityGroupCounts](../api/reportroot-getoffice365groupsactivitygroupcounts.md)</li><li>[getOffice365GroupsActivityStorage](../api/reportroot-getoffice365groupsactivitystorage.md)</li><li>[getOffice365GroupsActivityFileCounts](../api/reportroot-getoffice365groupsactivityfilecounts.md)</li></ul> |
| OneDriveActivity        | <ul><li>[getOneDriveActivityUserDetail](../api/reportroot-getonedriveactivityuserdetail.md)</li><li>[getOneDriveActivityUserCounts](../api/reportroot-getonedriveactivityusercounts.md)</li><li>[getOneDriveActivityFileCounts](../api/reportroot-getonedriveactivityfilecounts.md)</li></ul> |
| OneDriveUsage           | <ul><li>[getOneDriveUsageAccountDetail](../api/reportroot-getonedriveusageaccountdetail.md)</li><li>[getOneDriveUsageAccountCounts](../api/reportroot-getonedriveusageaccountcounts.md)</li><li>[getOneDriveUsageFileCounts](../api/reportroot-getonedriveusagefilecounts.md)</li><li>[getOneDriveUsageStorage](../api/reportroot-getonedriveusagestorage.md)</li></ul> |
| SharePointActivity      | <ul><li>[getSharePointActivityUserDetail](../api/reportroot-getsharepointactivityuserdetail.md)</li><li>[getSharePointActivityFileCounts](../api/reportroot-getsharepointactivityfilecounts.md)</li><li>[getSharePointActivityUserCounts](../api/reportroot-getsharepointactivityusercounts.md)</li><li>[getSharePointActivityPages](../api/reportroot-getsharepointactivitypages.md)</li></ul> |
| SharePointSiteUsage     | <ul><li>[getSharePointSiteUsageDetail](../api/reportroot-getsharepointsiteusagedetail.md)</li><li>[getSharePointSiteUsageFileCounts](../api/reportroot-getsharepointsiteusagefilecounts.md)</li><li>[getSharePointSiteUsageSiteCounts](../api/reportroot-getsharepointsiteusagesitecounts.md)</li><li>[getSharePointSiteUsageStorage](../api/reportroot-getsharepointsiteusagestorage.md)</li><li>[getSharePointSiteUsagePages](../api/reportroot-getsharepointsiteusagepages.md)</li></ul> |
| SfbActivity             | <ul><li>[getSkypeForBusinessActivityUserDetail](../api/reportroot-getskypeforbusinessactivityuserdetail.md)</li><li>[getSkypeForBusinessActivityCounts](../api/reportroot-getskypeforbusinessactivitycounts.md)</li><li>[getSkypeForBusinessActivityUserCounts](../api/reportroot-getskypeforbusinessactivityusercounts.md)</li></ul> |
| SfbDeviceUsage          | <ul><li>[getSkypeForBusinessDeviceUsageUserDetail](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md)</li><li>[getSkypeForBusinessDeviceUsageDistributionUserCounts](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md)</li><li>[getSkypeForBusinessDeviceUsageUserCounts](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md)</li></ul> |
| SfbOrganizerActivity    | <ul><li>[getSkypeForBusinessOrganizerActivityCounts](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md)</li><li>[getSkypeForBusinessOrganizerActivityUserCounts](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md)</li><li>[getSkypeForBusinessOrganizerActivityMinuteCounts](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md)</li></ul> |
| SfbParticipantActivity  | <ul><li>[getSkypeForBusinessParticipantActivityCounts](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md)</li><li>[getSkypeForBusinessParticipantActivityUserCounts](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md)</li><li>[getSkypeForBusinessParticipantActivityMinuteCounts](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md)</li></ul> |
| SfbP2PActivity          | <ul><li>[getSkypeForBusinessPeerToPeerActivityCounts](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md)</li><li>[getSkypeForBusinessPeerToPeerActivityUserCounts](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md)</li><li>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md)</li></ul> |
| YammerActivity          | <ul><li>[getYammerActivityUserDetail](../api/reportroot-getyammeractivityuserdetail.md)</li><li>[getYammerActivityCounts](../api/reportroot-getyammeractivitycounts.md)</li><li>[getYammerActivityUserCounts](../api/reportroot-getyammeractivityusercounts.md)</li></ul> |
| YammerDeviceUsage       | <ul><li>[getYammerDeviceUsageUserDetail](../api/reportroot-getyammerdeviceusageuserdetail.md)</li><li>[getYammerDeviceUsageDistributionUserCounts](../api/reportroot-getyammerdeviceusagedistributionusercounts.md)</li><li>[getYammerDeviceUsageUserCounts](../api/reportroot-getyammerdeviceusageusercounts.md)</li></ul> |
| YammerGroupsActivity    | <ul><li>[getYammerGroupsActivityDetail](../api/reportroot-getyammergroupsactivitydetail.md)</li><li>[getYammerGroupsActivityGroupCounts](../api/reportroot-getyammergroupsactivitygroupcounts.md)</li><li>[getYammerGroupsActivityCounts](../api/reportroot-getyammergroupsactivitycounts.md)</li></ul> |

## <a name="next-steps"></a>Nächste Schritte

Berichtsressourcen und APIs können Ihnen neue Möglichkeiten eröffnen, über die Sie mit Benutzer in Kontakt treten und ihre Erfahrungen mit Microsoft Graph verwalten können. So erhalten Sie weitere Informationen:

- Informieren Sie sich ausführlicher über die Methoden und Eigenschaften der Ressourcen, die für Ihr Szenario am hilfreichsten sind.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).
