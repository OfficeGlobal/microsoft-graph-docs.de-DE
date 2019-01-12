---
title: Arbeiten mit Gruppen in Microsoft Graph
description: Gruppen sind Auflistungen von Benutzern und anderen Hauptbenutzern, die den Zugriff auf Ressourcen in Microsoft-Diensten oder in Ihrer App gemeinsam nutzen. Microsoft Graph enthält APIs, die Sie zum Erstellen und Verwalten von verschiedenen Typen von Gruppen und Gruppenfunktionalitäten entsprechend Ihrem Szenario verwenden können. Für alle gruppenbezogenen Vorgänge in Microsoft Graph ist die Zustimmung durch einen Administrator erforderlich.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 031d67db4f0ad151175fc244aefdfd31615b221c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961687"
---
# <a name="working-with-groups-in-microsoft-graph"></a>Arbeiten mit Gruppen in Microsoft Graph

Gruppen sind Auflistungen von [Benutzern](user.md) und anderen Hauptbenutzern, die den Zugriff auf Ressourcen in Microsoft-Diensten oder in Ihrer App gemeinsam nutzen. Microsoft Graph enthält APIs, die Sie zum Erstellen und Verwalten von verschiedenen Typen von Gruppen und Gruppenfunktionalitäten entsprechend Ihrem Szenario verwenden können. Für alle gruppenbezogenen Vorgänge in Microsoft Graph ist die Zustimmung durch einen Administrator erforderlich.

> **Hinweis**: Gruppen können nur über Geschäfts- oder Schulkonten erstellt werden. Persönliche Microsoft-Konten unterstützen keine Gruppen.

| Typ              | Anwendungsfall | groupType | E-Mail-aktiviert | Mit aktivierter Sicherheit | Erstellung über API möglich? |
|-------------------|----------|-----------|--------------|------------------|--------------------------------|
| [Office 365-Gruppen](#office-365-groups) | Ermöglicht die Zusammenarbeit von Benutzern mit freigegebenen Microsoft-Onlineressourcen. | `["Unified"]` | `true` | `false` | Ja |
| [Sicherheitsgruppen](#security-groups-and-mail-enabled-security-groups) | Steuern des Benutzerzugriffs auf Ressourcen innerhalb der App. | `[]` | `false` | `true` | Ja |
| [E-Mail-aktivierte Sicherheitsgruppen](#security-groups-and-mail-enabled-security-groups) | Steuern des Benutzerzugriffs auf Ressourcen innerhalb der App mit einem freigegebenen Gruppenpostfach. | `[]` | `true` | `true` | Nein |
| Verteilergruppen | Verteilen von E-Mail-Nachrichten an die Mitglieder der Gruppe. Es wird empfohlen, dass Sie aufgrund der vielfältigeren Ressourcen Office 365-Gruppen verwenden. | `[]` | `true` | `false` | Nein |

## <a name="office-365-groups"></a>Office 365-Gruppen
Die Leistungsfähigkeit von Office 365-Gruppen liegt an der Zusammenarbeitsfunktion, die ideal für Personen geeignet ist, die an einem Projekt oder in einem Team zusammenarbeiten. Diese werden mit Ressourcen erstellt, die Mitglieder der Gruppe gemeinsam verwenden, darunter:

- Outlook-Unterhaltungen auflisten
- Outlook-Kalender
- SharePoint-Dateien
- OneNote-Notizbuch
- SharePoint-Teamwebsite
- Planner-Pläne
- Intune-Geräteverwaltung

### <a name="group-in-outlook-example"></a>Beispiel einer Gruppe in Outlook

Es folgt eine JSON-Darstellung von Gruppen in Outlook. 

```http

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "4c5ee71b-e6a5-4343-9e2c-4244bc7e0938",
    "deletedDateTime": null,
    "classification": "MBI",
    "createdDateTime": "2016-08-23T14:46:56Z",
    "description": "This is a group in Outlook",
    "displayName": "OutlookGroup101",
    "groupTypes": [
        "Unified"
    ],
    "mail": "outlookgroup101@service.microsoft.com",
    "mailEnabled": true,
    "mailNickname": "outlookgroup101",
    "preferredLanguage": null,
    "proxyAddresses": [
        "smtp:outlookgroup101@microsoft.onmicrosoft.com",
        "SMTP:outlookgroup101@service.microsoft.com"
    ],
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```
Weitere Informationen zu Office 365-Gruppen und der Administratorerfahrung finden Sie unter [Weitere Informationen zu Gruppen in Office 365](https://support.office.com/en-us/article/Learn-about-Office-365-groups-b565caa1-5c40-40ef-9915-60fdb2d97fa2).

## <a name="security-groups-and-mail-enabled-security-groups"></a>Sicherheitsgruppen und E-Mail-aktivierte Sicherheitsgruppen

Sicherheitsgruppen sind für das Steuern des Benutzerzugriffs auf Ressourcen gedacht. Durch Überprüfen, ob ein Benutzer ein Mitglied einer Sicherheitsgruppe ist, kann Ihre App Autorisierungsentscheidungen treffen, wenn dieser Benutzer versucht, auf sichere Ressourcen in Ihrer App zuzugreifen. Sicherheitsgruppen können Benutzer und andere Sicherheitsgruppen als Mitglieder haben.

E-Mail-aktivierte Sicherheitsgruppen werden auf die gleiche Weise wie Sicherheitsgruppen verwendet, weisen jedoch das zusätzliche Feature eines freigegebenen Postfachs für die Gruppen auf. E-Mail-aktivierte Sicherheitsgruppen können nicht über die API erstellt werden, aber andere Gruppenvorgänge funktionieren weiterhin.  E-Mail-aktivierte Sicherheitsgruppen sind schreibgeschützt. Weitere Informationen finden Sie im Exchange-Artikel  [Verwalten von E-Mail-aktivierten Sicherheitsgruppen](https://technet.microsoft.com/en-us/library/bb123521%28v=exchg.160%29.aspx).

### <a name="security-group-example"></a>Beispiel für eine Sicherheitsgruppe

Es folgt eine JSON-Darstellung einer Sicherheitsgruppe. 

```http
{
    "@odata.type": "#microsoft.graph.group",
    "id": "f87faa71-57a8-4c14-91f0-517f54645106",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2016-07-20T09:21:23Z",
    "description": "This group is a Security Group",
    "displayName": "SecurityGroup101",
    "groupTypes": [],
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "",
    "preferredLanguage": null,
    "proxyAddresses": [],
    "securityEnabled": true
}
```
## <a name="dynamic-membership"></a>Dynamische Mitgliedschaft 

Alle Typen von Gruppen können Regeln für dynamische Mitgliedschaft aufweisen, die automatisch Mitglieder zu der Gruppe basierend auf den Benutzereigenschaften hinzufügen oder darauf entfernen. Die Gruppe „Marketing-Mitarbeiter“ würde beispielsweise jeden Benutzer einschließen, für den die department-Eigenschaft auf „Marketing“ festgelegt ist, sodass neue Marketing-Mitarbeiter automatisch zu der Gruppe hinzugefügt werden, und Mitarbeiter, die die Abteilung verlassen, automatisch aus der Gruppe entfernt werden. Diese Regel kann im Feld „membershipRule“ während der Erstellung von Gruppen als `"membershipRule": 'user.department -eq "Marketing"'` festgelegt werden. GroupType muss auch `"DynamicMembership"` umfassen. Die folgende Anforderung erstellt eine neue Office 365-Gruppe für die Marketing-Mitarbeiter: 

```http
POST https://graph.microsoft.com/beta/groups
{
    "description": "Marketing department folks",
    "displayName": "Marketing department",
    "groupTypes": [
        "Unified",
        "DynamicMembership"
    ],
    "mailEnabled": true,
    "mailNickname": "marketing",
    "securityEnabled": false,
    "membershipRule": 'user.department -eq "Marketing"',
    "membershipRuleProcessingState": "on"
}
```

Weitere Informationen zum Verfassen von membershipRules finden Sie unter [Erstellen von attributbasierten Regeln für dynamische Gruppenmitgliedschaft in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-groups-dynamic-membership-azure-portal).

> **Hinweis**: Regeln für dynamische Mitgliedschaft erfordern eine Lizenz vom Mandanten auf der Ebene [Azure Active Directory Premium P1](https://azure.microsoft.com/en-us/pricing/details/active-directory/) oder höher.

## <a name="other-types-of-groups"></a>Andere Arten von Gruppen

Office 365-Gruppen in Yammer werden verwendet, um die Zusammenarbeit von Benutzern über Yammer-Beiträge zu ermöglichen. Diese Art von Gruppe kann über eine Leseanforderung zurückgegeben werden, auf die Beiträge kann jedoch nicht über die API zugegriffen werden. Wenn Yammer-Beiträge und Unterhaltungs-Feeds für eine Gruppe aktiviert sind, werden standardmäßige Office 365-Gruppenunterhaltungen deaktiviert. Weitere Informationen finden Sie unter [Yammer-Entwickler-API Dokumente](https://developer.yammer.com/docs).

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Mit Microsoft Graph können Sie die folgenden allgemeinen Vorgänge ausführen.

| **Anwendungsfälle**  | **REST-Ressourcen** | **Siehe auch** |
|:---------------|:--------|:----------|
| **Gruppenobjekt und Methoden** | | |
| Neue Gruppen erstellen, vorhandene Gruppen abrufen, die Eigenschaften für Gruppe aktualisieren und Gruppen löschen. Derzeit können nur Sicherheitsgruppen und Gruppen in Outlook über die API erstellt werden. | [Gruppe](group.md) | [Neue Gruppen erstellen](../api/group-post-groups.md) <br/> [Gruppen auflisten](../api/group-list.md) <br/> [Gruppen aktualisieren](../api/group-update.md) <br/> [Gruppen löschen](../api/group-delete.md) |
| **Methoden für Gruppenmitgliedschaft** | | |
| Mitglieder einer Gruppe auflisten und Mitglieder hinzufügen oder entfernen. | [user](user.md) <br/> [Gruppe](group.md)| [Mitglieder auflisten](../api/group-list-members.md) <br/> [Mitglied hinzufügen](../api/group-post-members.md) <br/> [Mitglied entfernen](../api/group-delete-members.md)|
| Bestimmen, ob ein Benutzer Mitglied einer Gruppe ist, alle Gruppen abrufen, bei denen der Benutzer Mitglied ist. | [user](user.md) <br/> [Gruppe](group.md)| [Mitgliedergruppen prüfen](../api/group-checkmembergroups.md) <br/> [Mitgliedergruppen abrufen](../api/group-getmembergroups.md)|
| Besitzer einer Gruppe auflisten und Besitzer hinzufügen oder entfernen. | [Benutzer](user.md) <br/> [Gruppe](group.md)| [Besitzer auflisten](../api/group-list-members.md) <br/> [Mitglied hinzufügen](../api/group-post-members.md) <br/> [Mitglied entfernen](../api/group-delete-members.md)|
