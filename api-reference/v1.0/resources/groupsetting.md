---
title: groupSetting-Ressourcentyp
description: Gruppeneinstellungen steuern Verhalten wie blockierte Wortlisten für Gruppenanzeigenamen oder ob Gastbenutzer Gruppenbesitzer sein können.
ms.openlocfilehash: 16eb67e717fb151a627961176b1409e8426e3178
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016881"
---
# <a name="groupsetting-resource-type"></a>groupSetting-Ressourcentyp

Gruppeneinstellungen steuern Verhalten wie blockierte Wortlisten für Gruppenanzeigenamen oder ob Gastbenutzer Gruppenbesitzer sein können.

Gruppeneinstellungen können basierend auf den verfügbaren [groupSettingTemplates](groupsettingtemplate.md) erstellt werden, und die Standardwerte können geändert werden. Diese Einstellungen regeln Gruppenverhalten auf mandantenweiter Ebene oder für eine bestimmte Gruppe. Wenn die gleiche Einstellung sowohl mandantenweit als auch für eine bestimmte Gruppe definiert ist, überschreibt die Einstellung auf Gruppierungsebene die mandantenweite Einstellung.  So ermöglicht die mandantenweite Einstellung Gästen möglicherweise, von vorhandenen Mitgliedern der Gruppe eingeladen zu werden, wobei eine einzelne Gruppeneinstellung dies jedoch überschreiben und nicht zulassen kann, das Gäste von Mitgliedern der Gruppe eingeladen werden. Gruppeneinstellungen regeln nur das Gruppenverhalten in Office 365.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[Einstellung erstellen](../api/groupsetting-post-groupsettings.md) | [groupSetting](groupsetting.md) |Erstellen Sie eine Einstellungsobjekt basierend auf einer groupSettingTemplate. Die POST-Anforderung muss settingValues für alle Einstellungen bereitstellen, die in der Vorlage definiert sind. |
|[Einstellung abrufen](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts. |
|[Einstellungen auflisten](../api/groupsetting-list.md) | [groupSetting](groupsetting.md)-Sammlung | Listet Eigenschaften aller Einstellungsobjekte auf. |
|[Einstellung aktualisieren](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | groupsetting-Objekt wird aktualisiert. |
|[Einstellung löschen](../api/groupsetting-delete.md) | Keine | Löscht ein Einstellungsobjekt. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|displayName|Zeichenfolge| Anzeigename für diese Gruppe von Einstellungen, der aus der zugeordneten Vorlage stammt. |
|id|Zeichenfolge| Eindeutiger Bezeichner für diese Einstellungen. Schreibgeschützt. |
|templateId|Zeichenfolge| Eindeutiger Bezeichner für die Vorlage, die zum Erstellen dieser Gruppe von Einstellungen verwendet wird. Schreibgeschützt. |
|values|[settingValue](settingvalue.md)-Sammlung| Sammlung von Name/Wert-Paaren. Muss alle Einstellungen, die in dieser Vorlage definiert sind, enthalten und festlegen. |

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->