---
title: Ressourcentyp Einstellungen
description: 'Den aktuellen benutzereinstellungen. '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 107ec7c425e4818f9233755e54d867b07087aa3c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805020"
---
# <a name="settings-resource-type"></a>Ressourcentyp Einstellungen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Den aktuellen benutzereinstellungen. Informationen zum Abrufen oder Aktualisieren von benutzereinstellungen, finden Sie unter [Abrufen von Einstellungen](../api/user-get-settings.md) und [Einstellungen aktualisieren](../api/user-update-settings.md).

Diese Ressource unterstützt Folgendes:

- Überprüfen, ob ein Benutzer und die Organisation des Benutzers zu Content-Erkennung beitragen.
- Deaktivieren oder Aktivieren der Content-Erkennung für bestimmte Benutzer. Dadurch wird deaktiviert, Dokumente in Office eingegangen wird.

## <a name="methods"></a>Methoden
| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen der Benutzereinstellungen](../api/user-get-settings.md) |[Einstellungen](../resources/user-settings.md)| Rufen Sie die Einstellungen für Benutzer und Organisation. |
|[Aktualisieren von benutzereinstellungen](../api/user-update-settings.md) |[Einstellungen](../resources/user-settings.md)| Aktualisieren Sie die aktuellen benutzereinstellungen. |

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
