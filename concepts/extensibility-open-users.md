---
title: Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen
description: 'Sie werden durch ein Beispiel geführt, um die Verwendung *offener Erweiterungen* zu veranschaulichen. '
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 69b0918dba3159a552e2b00d4f54b21e67d017e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867263"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a>Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen
Sie werden durch ein Beispiel geführt, um die Verwendung *offener Erweiterungen* zu veranschaulichen. 

Angenommen, Sie erstellen eine Anwendung, die auf vielen verschiedenen Clientplattformen, z. B. Desktop und Mobil, verfügbar ist.  Sie möchten zulassen, dass Benutzer ihre eigene Benutzeroberfläche konfigurieren, damit diese konsistent ist, unabhängig davon, mit welchem Gerät sie sich bei der App anmelden. Dies ist eine allgemeine Anforderung für die meisten Apps. 

In diesem Szenario erlernen Sie Folgendes:

1. Hinzufügen einer offenen Erweiterung, die einige Roamingprofilinformationen über den Benutzer darstellt.
2. Abfragen des Benutzers und Zurückgeben des Roamingprofils.
3. Ändern der Roamingprofilinformationen des Benutzers (der Wert der offenen Erweiterung).
4. Löschen der Roamingprofilinformationen des Benutzers.

>**Hinweis:** In diesem Thema wird gezeigt, wie offenen Erweiterungen in einer *user*-Ressource hinzugefügt, gelesen, aktualisiert und gelöscht werden.  Diese Methoden werden auch für die Ressourcentypen *administrativeUnit*, *contact*, *device*, *event*, *group*, *group event*, *group post* und *organizaton* unterstützt.  
Aktualisieren Sie einfach die Beispielanforderungen unter Verwendung dieser Ressourcentypen. Die in den Beispielen dargestellten Antworten sind aus Platzgründen möglicherweise abgeschnitten. 

## <a name="1-add-roaming-profile-information"></a>1. Hinzufügen von Roamingprofilinformationen
Der Benutzer meldet sich bei der App an und konfiguriert das Aussehen und Verhalten der App.  Diese App-Einstellungen sind roamingfähig, der Benutzer erhält also dieselbe Oberfläche, ganz gleich, mit welchem Gerät er sich bei der App anmeldet.  Hier sehen Sie, wie die Roamingprofilinformationen zu einer Benutzerressource hinzugefügt werden.

##### <a name="request"></a>Anforderung
```http
POST https://graph.microsoft.com/v1.0/me/extensions
Content-type: application/json
{
    "@odata.type":"microsoft.graph.openTypeExtension",
    "extensionName":"com.contoso.roamingSettings",
    "theme":"dark",
    "color":"purple",
    "lang":"Japanese"
}
```
##### <a name="response"></a>Antwort
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a>2. Abrufen von Roamingprofilinformationen
Wenn sich der Benutzer von einem anderen Gerät aus bei der App anmeldet, kann die App die Profildetails des Benutzers und auch die Roamingeinstellungen abrufen. Dies kann durch Abrufen der Benutzerressource und Erweitern der Erweiterungsnavigationseigenschaft erfolgen.

##### <a name="request"></a>Anforderung
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
##### <a name="response"></a>Antwort
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420

{
    "id": "84b80893-8749-40a3-97b7-68513b600544",
    "displayName": "John Smith",
    "mail": "john@contoso.com",
    "mobilePhone": "1-555-6589",
    "extensions": [
        {
            "@odata.type": "#microsoft.graph.openTypeExtension",
            "extensionName": "com.contoso.roamingSettings",
            "id": "com.contoso.roamingSettings",
            "theme": "dark",
            "color": "purple",
            "lang": "Japanese"
        }
    ]
}
```
>**Hinweis:** Wenn Sie mehrere Erweiterungen haben, können Sie nach der *ID* filtern, um die gewünschte Erweiterung zu erhalten.

## <a name="3-change-roaming-profile-information"></a>3. Ändern der Roamingprofilinformationen
Der Benutzer kann seine Roamingprofilinformationen ändern.  Diese Aktualisierung kann über eine ```PATCH``` im Wert der offenen Erweiterung erfolgen. 

##### <a name="request"></a>Anforderung
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

##### <a name="response"></a>Antwort
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a>4. Löschen der Roamingprofilinformationen eines Benutzers
Der Benutzer entscheidet, dass er kein Roamingprofil mehr benötigt, und löscht es. Dies kann über eine ```DELETE```-Anforderung im Wert der offenen Erweiterung erfolgen.

##### <a name="request"></a>Anforderung
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a>Antwort
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](extensibility-overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](extensibility-schema-groups.md)
- [openTypeExtension-Ressourcentyp](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [Offene Erweiterung erstellen](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [Offene Erweiterung abrufen](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [Offene Erweiterung aktualisieren](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [Offene Erweiterung löschen](/graph/api/opentypeextension-delete?view=graph-rest-1.0)
