---
title: Ressourcentyp Einstellungen
description: 'Den aktuellen benutzereinstellungen. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521096"
---
# <a name="settings-resource-type"></a>Ressourcentyp Einstellungen

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Den aktuellen benutzereinstellungen. Informationen zum Abrufen oder Aktualisieren von benutzereinstellungen, finden Sie unter [Abrufen von Einstellungen](../api/user-get-settings.md) und [Einstellungen aktualisieren](../api/user-update-settings.md).

Diese Ressource unterstützt Folgendes:

- Überprüfen, ob ein Benutzer und die Organisation des Benutzers zu Content-Erkennung beitragen.
- Deaktivieren oder Aktivieren der Content-Erkennung für bestimmte Benutzer. Dadurch wird deaktiviert, Dokumente in Office eingegangen wird.

## <a name="methods"></a>Methoden
| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|Abrufen der Benutzereinstellungen |[](../resources/user-settings.md) Einstellungen| Rufen Sie die Einstellungen für Benutzer und Organisation. |
|[Aktualisieren von benutzereinstellungen](../api/user-update-settings.md) |[](../resources/user-settings.md) Einstellungen| Aktualisieren Sie die aktuellen benutzereinstellungen. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Boolescher Wert|Bei Festlegung auf "true", das Delegieren des Zugriffs für des Benutzers ist [Trend](insights-trending.md) API deaktiviert. Bei Festlegung auf true fest, Dokumente in des Benutzers Office eingegangen sind deaktiviert. Bei Festlegung auf "true", die Relevanz des Inhalts in Office 365, beispielsweise in vorgeschlagene in SharePoint – Startseite angezeigt, und die Ansicht Discover in OneDrive für Unternehmen betroffen ist. Benutzer können diese Einstellung in [Office eingegangen](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout)steuern. |
|contributionToContentDiscoveryAsOrganizationDisabled|Boolescher Wert|Gilt für die [Einstellung der Organisation](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) Steuern des Zugriffs auf die [Trend](insights-trending.md) -API-Delegaten. Wenn nicht auf True festgelegt, der Organisation auf Office eingegangen zugreifen kann. Die Relevanz des Inhalts in Office 365, beispielsweise in vorgeschlagene in SharePoint-Startseite und in der Ansicht Discover in OneDrive für Unternehmen angezeigt, ist für die gesamte Organisation betroffen. Diese Einstellung ist schreibgeschützt und kann nur von Administratoren in der [SharePoint-Verwaltungskonsole](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US)geändert werden.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/user-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
