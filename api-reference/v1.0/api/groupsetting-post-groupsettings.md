---
title: Erstellen einer Gruppeneinstellung
description: Verwenden Sie diese API zum Erstellen einer neuen Einstellung, basierend auf den Vorlagen, die in groupSettingTemplates zur Verfügung stehen. Diese Einstellungen können auf Mandantenebene oder auf Gruppenebene erfolgen. Die Erstellungsanforderung muss settingValues für alle Einstellungen bereitstellen, die in der Vorlage definiert sind. Bei gruppenspezifischen Einstellungen kann nur die Einstellung, die regelt, ob die Mitglieder einer Gruppe Gastbenutzer einladen können, festgelegt werden. Dies steuert dieses Verhalten, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe allgemein verfügbar ist.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e87e34f5816818c25cef5768c08ab8f7c73a3a0f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923145"
---
# <a name="create-a-group-setting"></a>Erstellen einer Gruppeneinstellung

Verwenden Sie diese API zum Erstellen einer neuen Einstellung, basierend auf den Vorlagen, die in [groupSettingTemplates](../resources/groupsettingtemplate.md) zur Verfügung stehen. Diese Einstellungen können auf Mandantenebene oder auf Gruppenebene erfolgen. Die Erstellungsanforderung muss [settingValues](../resources/settingvalue.md) für alle Einstellungen bereitstellen, die in der Vorlage definiert sind. Bei gruppenspezifischen Einstellungen kann nur die Einstellung, die regelt, ob die Mitglieder einer Gruppe Gastbenutzer einladen können, festgelegt werden. Dies steuert dieses Verhalten, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe allgemein verfügbar ist.

Verwenden Sie eine Liste der Vorlagen und die Eigenschaften, die sie in v1. 0 unterstützen, einer [GroupSettingTemplate Abfrage](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0) (für Beta Endpunkte, Anruf [DirectorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a>Anforderungsheader

| Name | Beschreibung |
|:---------------|:----------|
| Authorization | Bearer {token}. Erforderlich. |
| Content-Type | application/json |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des [groupSetting](../resources/groupsetting.md)-Objekts an. Der Anzeigenamen für die Einstellung wird jedoch basierend auf dem Namen der referenzierten Einstellungsvorlage festgelegt.

## <a name="response"></a>Antwort

Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `201 Created` und das [groupSetting](../resources/groupsetting.md)-Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
Geben Sie im Anforderungstext eine JSON-Darstellung des [groupSetting](../resources/groupsetting.md)-Objekts an.
##### <a name="response"></a>Antwort

Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
