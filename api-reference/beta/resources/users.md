---
title: Arbeiten mit Benutzern in Microsoft Graph
description: Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b98bdd3f84171823942b3a48dd49a8993597a5ee
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572178"
---
# <a name="working-with-users-in-microsoft-graph"></a>Arbeiten mit Benutzern in Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.

Sie können auf zwei Arten über Microsoft Graph auf Benutzer zugreifen:

- Anhand der ID, `/users/{id}` 
- Anhand des `/me`-Alias für den angemeldeten Benutzer, welcher `/users/{signed-in user's id}` entspricht

## <a name="authorization"></a>Autorisierung
Für den Zugriff auf Benutzervorgänge ist eine der folgenden [Berechtigungen](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) erforderlich. Die ersten drei Berechtigungen können einer App durch einen Benutzer gewährt werden. Die übrigen können der App nur durch einen Administrator gewährt werden.

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="common-properties"></a>Allgemeine Eigenschaften

Im Folgenden werden standardmäßige Eigenschaften dargestellt, die beim Abrufen eines Benutzers oder beim Auflisten von Benutzern zurückgegeben werden. Diese stellen eine Teilmenge aller verfügbaren Eigenschaften. Verwenden Sie zum Abrufen weiterer Benutzereigenschaften den `$select`-Abfrageparameter. 

|Eigenschaft |Beschreibung |
|:----------|:-------------|
|id | Die eindeutige ID des Benutzers.|
|businessPhones | Telefonnummern des Benutzers.|
|displayName | Der Name des Benutzers, der im Adressbuch angezeigt wird.|
|givenName| Der Vorname des Benutzers. |
|jobTitle | Die Position des Benutzers.|
|mail| Die E-Mail-Adresse des Benutzers. |
|mobilePhone | Die Mobiltelefonnummern des Benutzers.|
|officeLocation | Der Bürostandort des Benutzers.|
|preferredLanguage | Die vom Benutzer bevorzugte Sprache.|
|surname| Der Nachname des Benutzers. |
|mail| Die E-Mail-Adresse des Benutzers. |
|photo| Das Profilfoto des Benutzers. |
|userPrincipalName| Der Benutzerprinzipalname. |

Weitere Informationen und eine Liste aller Eigenschaften finden Sie unter [user](user.md)-Objekt.

## <a name="common-operations"></a>Allgemeine Vorgänge
>**Hinweis:** Einige dieser Vorgänge erfordern zusätzliche Berechtigungen.

| Pfad    | Beschreibung |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | Listet die Benutzer in der Organisation auf. |
|[`/users/{id}`](../api/user-get.md) | Ruft einen bestimmten Benutzer anhand der ID ab. |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| Ruft das Profilfoto des Benutzers ab. |
|[`/users/{id}/manager`](../api/user-list-manager.md) | Ruft den Vorgesetzten des Benutzers ab. |
|[`/users/{id}/messages`](../api/user-list-messages.md)| Listet die E-Mails des Benutzers im primären Posteingang auf. |
|[`/users/{id}/events`](../api/user-list-events.md) | Listet bevorstehende Ereignisse des Benutzers im Kalender auf. |
|[`/users/{id}/drive`](../api/drive-get.md)| Ruft den OneDrive-Dateispeicher des Benutzers ab. |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| Listet die Gruppen auf, deren Mitglied der Benutzer ist. |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| Listet die Microsoft Teams auf, deren Mitglied der Benutzer ist. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
