---
title: Einstellungen für Updates
description: 'Aktualisieren Sie die Eigenschaften des Settings-Objekts. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d21d7fb26945e4a46fdf877bb5911aba0621ce3b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508762"
---
# <a name="update-settings"></a>Einstellungen für Updates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Eigenschaften des [Settings](../resources/user-settings.md) -Objekts. Benutzer in derselben Organisation können unterschiedliche Einstellungen basierend auf ihrer Präferenz oder auf den Richtlinien der Organisation verfügen. Um die aktuelle Einstellungen abrufen, finden Sie in der [aktuellen benutzereinstellungen](user-get-settings.md). 

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | User.ReadWrite User.ReadWrite.All   |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | User.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung

```http
PATCH https://graph.microsoft.com/beta/me/settings
```

Fordern Sie mit einer 'Benutzer-Id"oder"UserPrincipalName"ist nur verfügbar, durch den Benutzer oder von einem Benutzer mit den Berechtigungen User.ReadWrite.All. Weitere Informationen finden Sie unter [Berechtigungen](/graph/permissions-reference). 

```http
PATCH https://graph.microsoft.com/beta/users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a>Anforderungsheader

| Kopfzeile       | Wert|
|:-----------|:------|
| Authorization  | Bearer {token}. Erforderlich.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Boolescher Wert|"True" eingestellt deaktiviere Delegieren des Zugriffs auf [Trending](../resources/insights-trending.md) API und Zugriff auf Dokumente in Office eingegangen für den Benutzer zu deaktivieren. Einstellung auch auf True wirkt sich auf die Relevanz des Inhalts angezeigt in Office 365 – beispielsweise vorgeschlagene in SharePoint-Startseite und in der Ansicht Discover in OneDrive für Unternehmen weniger relevante Ergebnisse anzeigen. Diese Einstellung entspricht dem Steuerelementzustand in [Office ausführlicher behandelt](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).|

## <a name="example"></a>Beispiel 

##### <a name="request"></a>Anforderung

Es folgt eine Beispiel für eine Anforderung zum Melden Sie sich einen Benutzer von Delve und seinen Beitrag auf Content Relevanz für die gesamte Organisation zu deaktivieren.

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a>Batchanforderung

Es ist auch möglich, melden Sie sich mehrere Benutzer aus Delve und Beitrags auf Content Relevanz für die gesamte Organisation über eine Batchanforderung deaktivieren.
Weitere Informationen finden Sie unter [JSON Batchverarbeitung](/graph/json-batching).

**Wichtig**: nur Mitglieder der Rollengruppe [Organisationsverwaltung](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) mehrere Benutzer aktualisiert werden können. 


<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-update-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
