---
title: Berechtigungen
description: 'Veröffentlichen einer app mit dem Microsoft-Teams, apps Katalog. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 656b4a148f1d53cb44e303265af5624ccd1e423b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932924"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a>Veröffentlichen von apps in Ihrer Organisation app-Katalog

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Veröffentlichen einer [app](../resources/teamsapp.md) mit dem Microsoft-Teams, apps Katalog. Diese API veröffentlicht insbesondere die app in Ihrer Organisation-Katalog (die Mandanten-app-Katalog); die erstellte Ressource müssen `distributionMethod`  =  `organization`.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Hinweis:** Nur globale Administratoren können diese API aufrufen. 

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)|
|:----------------------------------     |:-------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | AppCatalog.ReadWrite.All |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt|
| Anwendung                            | Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a>Anforderungsheader

| Header        | Wert           |
|:--------------|:--------------  |
| Authorization | Bearer {token}. Erforderlich.  |
| Content-Type  | Anwendung/zip |

## <a name="request-body"></a>Anforderungstext

Manifest Teams Zip-Nutzlast. Zip-Datei [finden Sie unter Erstellen eines app-Pakets](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)für Teams fest. Sie können keine app für eine Organisation erstellen, die die gleiche manifest-ID als einer anderen Anwendung in der Organisation hat.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und ein [TeamsCatalogApp](../resources/teamsapp.md) -Objekt.

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Informationen dazu, wie Sie eine Microsoft-Teams Anwendung Zip-Datei erstellen finden Sie unter [Erstellen eines app-Pakets](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). 

### <a name="response"></a>Antwort

```
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```
