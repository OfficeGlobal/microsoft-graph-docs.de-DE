---
title: Arbeiten mit Benutzern in Microsoft Graph
description: Mit Microsoft Graph können Sie überzeugende App-Erfahrung basierend auf Benutzern, Beziehungen mit anderen Benutzern und Gruppen, und E-Mails, Kalender und Dateien bieten.
localization_priority: Priority
ms.openlocfilehash: d9b699c008186f165a8be43ab4254213697710dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860830"
---
# <a name="working-with-users-in-microsoft-graph"></a>Arbeiten mit Benutzern in Microsoft Graph

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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

| Eigenschaft | Beschreibung |
|----------|-------------|
| displayName | Der Name des Benutzers, der im Adressbuch angezeigt wird.|
|givenName| Der Vorname des Benutzers. |
|surname| Der Nachname des Benutzers. |
|mail| Die E-Mail-Adresse des Benutzers. |
|photo| Profil-Foto des Benutzers. |

Weitere Informationen und eine Liste aller Eigenschaften finden Sie unter [user](user.md)-Objekt.

## <a name="common-operations"></a>Allgemeine Vorgänge
>**Hinweis:** Einige dieser Vorgänge erfordern zusätzliche Berechtigungen.

| Pfad    | Beschreibung |
|---------|-------------|
|[`/users`](../api/user-list.md) | Listet die Benutzer in der Organisation auf. |
|[`/users/{id}`](../api/user-get.md) | Ruft einen bestimmten Benutzer anhand der ID ab. |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| Ruft das Profilfoto des Benutzers ab. |
|[`/users/{id}/manager`](../api/user-list-manager.md) | Ruft den Vorgesetzten des Benutzers ab. |
|[`/users/{id}/messages`](../api/user-list-messages.md)| Listet die E-Mails des Benutzers im primären Posteingang auf. |
|[`/users/{id}/events`](../api/user-list-events.md) | Listet bevorstehende Ereignisse des Benutzers im Kalender auf. |
|[`/users/{id}/drive`](../api/drive-get.md)| Ruft den OneDrive-Dateispeicher des Benutzers ab. |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| Listet die Gruppen auf, deren Mitglied der Benutzer ist. |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| Listet die Microsoft-Teams, die der Benutzer Mitglied ist. |
