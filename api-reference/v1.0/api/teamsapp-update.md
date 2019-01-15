---
title: Berechtigungen
description: 'Aktualisieren einer app zuvor in der Microsoft-Teams, app-Katalog veröffentlicht. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b89380a423bf01f6a2bd7e56086cc9290be094cb
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016625"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a>Aktualisieren von apps in Ihrer Organisation app-Katalog veröffentlicht



Aktualisieren einer [app](../resources/teamsapp.md) veröffentlicht zuvor in der Microsoft-Teams, app-Katalog. Diese API aktualisiert speziell eine app in Ihrer Organisation app-Katalog (die Mandanten-app-Katalog) veröffentlicht. Geben Sie zum Veröffentlichen in Ihrer Organisation app-Katalog `organization` als die **DistributionMethod** in der [TeamsCatalogApp](../resources/teamsapp.md) -Ressource.

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
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a>Anforderungsheader

| Header        | Wert           |
|:--------------|:--------------  |
| Authorization | Bearer {token}. Erforderlich.  |
| Content-Type  | Anwendung/zip |

## <a name="request-body"></a>Anforderungstext

Manifest Teams Zip-Nutzlast: Für Teams Anwendung zip-Datei [Erstellen eines app-Pakets finden Sie unter](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

>**Hinweis:** Verwenden Sie die ID aus der [Liste apps veröffentlicht](./teamsapp-list.md) Aufruf für zurückgegeben, auf um die app zu verweisen, die Sie aktualisieren möchten. Verwenden Sie nicht die in der Manifestdatei der app Zip-Paket-ID ein.

## <a name="response"></a>Antwort

```
HTTP/1.1 204 No Content
```

## <a name="example"></a>Beispiel

### <a name="request"></a>Anforderung

```
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Für Teams Anwendung zip-Datei [finden Sie unter Erstellen von app-Paket](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

### <a name="response"></a>Antwort

```
HTTP/1.1 204 No Content
```
