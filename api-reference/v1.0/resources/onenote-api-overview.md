---
title: Verwenden der OneNote-REST-API
description: Microsoft Graph können Ihre app autorisierten Zugriff auf eines Benutzers OneNote-Notizbücher, Abschnitte und Seiten in einem persönlichen oder Organisation Konto zu erhalten. Mit der entsprechenden delegiert, oder Berechtigungen für die Anwendung, Ihre app die OneNote-Daten des angemeldeten Benutzers oder jeder Benutzer in einem Mandanten zugreifen können.
localization_priority: Priority
ms.openlocfilehash: 1f78437b115825b8fd1ad2fdf14862543977d886
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866521"
---
# <a name="use-the-onenote-rest-api"></a>Verwenden der OneNote-REST-API

Microsoft Graph können Ihre app autorisierten Zugriff auf eines Benutzers OneNote-Notizbücher, Abschnitte und Seiten in einem persönlichen oder Organisation Konto zu erhalten. Mit den [entsprechenden Berechtigungen für delegierte oder Anwendung](/graph/permissions-reference#notes-permissions)kann Ihre app die OneNote-Daten des angemeldeten Benutzers oder jeder Benutzer in einem Mandanten zugreifen.

## <a name="root-url"></a>Stamm-URL
Die Stamm-URL des OneNote-Diensts verwendet das folgende Format für alle Aufrufe der OneNote-API:
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
Die `version` Segment in der URL darstellt, die Version von Microsoft Graph, die Sie verwenden möchten:

- Setzen Sie `v1.0` für stabilen Produktionscode.
- Setzen Sie `beta`, wenn Sie ein Feature testen möchten, das sich noch in der Entwicklung befindet. Features und Funktionen in der Beta-Endpunkt möglicherweise ändern. Es wird nicht empfohlen, für die Verwendung in Ihrem Produktionscode.

Der Speicherort kann Benutzer Notizbücher auf Office 365 oder Consumer OneDrive, Gruppe Notebooks oder SharePoint-Website gehosteten Team Notizbücher auf Office 365 sein. 

![OneNote-API-Entwicklung Stapel](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>Benutzer-Notizbüchern
Verwenden Sie den Zugriff auf persönliche Notizbücher auf Consumer OneDrive oder OneDrive für Unternehmen eine der folgenden URLs:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- Setzen Sie `me` für OneNote-Inhalte, auf die der aktuelle Benutzer zugreifen kann (eigene und freigegebene Inhalte).
- Setzen Sie `users/{id}` für OneNote-Inhalte, die der (in der URL) angegebene Benutzer für den aktuellen Benutzer freigegeben hat. Verwenden Sie die [Benutzer](users.md) API.
> **Hinweis:** Sie können die Benutzer-IDs abrufen, indem Sie tätigen eine GET-Anforderung auf `https://graph.microsoft.com/v1.0/users`.

### <a name="group-notebooks"></a>Gruppe-Notizbüchern
Um Notizbücher zugreifen, die eine Gruppe gehören, verwenden Sie die folgenden dienststamm-URL:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint-Website-Notizbüchern

Um Notizbücher zugreifen, die SharePoint-Teamwebsite gehören, verwenden Sie die folgenden dienststamm-URL:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

