---
title: Erstellen einer Einstellung directory
description: Verwenden Sie diese API, um eine neue Einstellung, basierend auf den in DirectorySettingTemplates verfügbaren Vorlagen erstellen. Diese Einstellungen kann die Mandanten-Ebene oder auf Objektebene (derzeit nur für Gruppen). Die Anforderung zum Erstellen eines muss EinstellenWerte für alle in der Vorlage definierten Einstellungen angeben. Für die Gruppe-spezifischen Einstellungen kann die Option nur die Einstellung steuern, ob Mitglieder einer Gruppe Gastbenutzer einladen können festgelegt werden. Dies wird dieses Verhalten gesteuert, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe im Allgemeinen verfügbar ist.
localization_priority: Normal
ms.openlocfilehash: 692ca0d68522b5b268e9ee670c694e5a5c6bee90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848720"
---
# <a name="create-a-directory-setting"></a>Erstellen einer Einstellung directory

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwenden Sie diese API, um eine neue Einstellung, basierend auf den in DirectorySettingTemplates verfügbaren Vorlagen erstellen. Diese Einstellungen kann die Mandanten-Ebene oder auf Objektebene (derzeit nur für Gruppen). Die Anforderung zum Erstellen eines muss EinstellenWerte für alle in der Vorlage definierten Einstellungen angeben. Für die Gruppe-spezifischen Einstellungen kann die Option nur die Einstellung steuern, ob Mitglieder einer Gruppe Gastbenutzer einladen können festgelegt werden. Dies wird dieses Verhalten gesteuert, sobald die Möglichkeit zum Hinzufügen von Gastbenutzern zu einer Gruppe im Allgemeinen verfügbar ist.

> **Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird. Die Version /v1.0 dieser API wurde in *Create GroupSettings*umbenannt.

Eine Liste der Vorlagen und die Eigenschaften, die sie in der Betaversion unterstützen, verwenden Sie eine [DirectorySettingTemplate Abfrage](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta). (Für v1. 0-Endpunkte, rufen Sie [GroupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)


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
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.  Jedoch wird der Anzeigename für die Einstellung basierend auf den Vorlagennamen referenzierten Einstellungen festgelegt werden.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Code und [Verzeichnisberechtigungen](../resources/directorysetting.md) Antwortobjekt im Antworttext.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Verzeichnisberechtigungen](../resources/directorysetting.md) -Objekts.
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
