---
title: groupSettingTemplate-Ressourcentyp
description: Gruppeneinstellungsvorlagen stellen systemdefinierte Einstellungen dar, die für den Mandanten verfügbar sind. Gruppeneinstellungen können basierend auf den verfügbaren **groupSettingTemplates** erstellt werden, und die Standardwerte können geändert werden. Gruppeneinstellungsvorlagen können nicht erstellt, aktualisiert oder gelöscht werden. Diese Einstellungen können mandantenweite Einstellungen oder bestimmte Gruppeneinstellungen darstellen. Die derzeit einzig verfügbaren Vorlagen beziehen sich auf Office 365-Gruppen und umfassen Einstellungen dazu, ob Benutzer Gruppen erstellen oder Gäste von außerhalb der Organisation einladen können, Mitglieder einer Gruppe zu werden.
localization_priority: Normal
ms.openlocfilehash: c2e6b465226b8c1c69438fab37d874735e89ac52
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859346"
---
# <a name="groupsettingtemplate-resource-type"></a>groupSettingTemplate-Ressourcentyp

Gruppeneinstellungsvorlagen stellen systemdefinierte Einstellungen dar, die für den Mandanten verfügbar sind. [Gruppeneinstellungen](groupsetting.md) können basierend auf den verfügbaren **groupSettingTemplates** erstellt werden, und die Standardwerte können geändert werden. Gruppeneinstellungsvorlagen können nicht erstellt, aktualisiert oder gelöscht werden. Diese Einstellungen können mandantenweite Einstellungen oder bestimmte Gruppeneinstellungen darstellen. Die derzeit einzig verfügbaren Vorlagen beziehen sich auf Office 365-Gruppen und umfassen Einstellungen dazu, ob Benutzer Gruppen erstellen oder Gäste von außerhalb der Organisation einladen können, Mitglieder einer Gruppe zu werden.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[Get groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | Liest die spezifischen Eigenschaften eines vom System definierten groupSettingTemplate-Objekts. |
|[List groupSettingTemplate](../api/groupsettingtemplate-list.md) | [Sammlung von groupSettingTemplate](groupsettingtemplate.md) |Listet alle der vom System definierten groupSettingTemplate-Objekte auf.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|description|Zeichenfolge| Beschreibung der Vorlage. |
|displayName|Zeichenfolge| Anzeigename der Vorlage. |
|id|Zeichenfolge| Der eindeutige Bezeichner für die Vorlage. Schreibgeschützt.|
|values|[settingTemplateValue](settingtemplatevalue.md)-Sammlung| Sammlung von settingTemplateValues, die den Satz der verfügbaren Einstellungen, Standardwerte und Typen auflistet, die diese Vorlage bilden. |

## <a name="relationships"></a>Beziehungen

Keine.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
