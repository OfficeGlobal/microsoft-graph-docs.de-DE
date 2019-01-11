---
title: Ressourcentyp directorySettingTemplate
description: Verzeichnis Einstellung Vorlagen darstellen, die dem Mandanten verfügbaren systemdefinierte Einstellungen. Directory-Einstellungen können anhand der verfügbaren DirectorySettingTemplates und Werte geändert voreingestellten Standardwerte von erstellt werden. Verzeichnis Einstellung Vorlagen können nicht erstellt, aktualisiert oder gelöscht werden. Diese Einstellungen können Mandanten geltende Einstellungen darstellen, oder Sie können bestimmte Entität Einstellungen darstellen.  Derzeit nur verfügbaren Vorlagen gelten für Office-Gruppen und umfassen Einstellungen wie gibt an, ob Benutzer Gruppen erstellen oder Gäste außerhalb der Organisation, die Mitglied einer Gruppe werden einladen können.
localization_priority: Normal
ms.openlocfilehash: e0df923854059723ee83380f7aa0f6425cf2afb9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806146"
---
# <a name="directorysettingtemplate-resource-type"></a>Ressourcentyp directorySettingTemplate

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verzeichnis Einstellung Vorlagen darstellen, die dem Mandanten verfügbaren systemdefinierte Einstellungen. [Directory-Einstellungen](directorysetting.md) können anhand der verfügbaren DirectorySettingTemplates und Werte geändert voreingestellten Standardwerte von erstellt werden. Verzeichnis Einstellung Vorlagen können nicht erstellt, aktualisiert oder gelöscht werden. Diese Einstellungen können Mandanten geltende Einstellungen darstellen, oder Sie können bestimmte Entität Einstellungen darstellen.  Derzeit nur verfügbaren Vorlagen gelten für Office-Gruppen und umfassen Einstellungen wie gibt an, ob Benutzer Gruppen erstellen oder Gäste außerhalb der Organisation, die Mitglied einer Gruppe werden einladen können.

> **Hinweis**: die /beta Version von dem Ressourcentyp DirectorySettingTemplate gilt nur für Gruppen. Die Version /v1.0 wurde in GroupSettingTemplate umbenannt.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von directorySettingTemplate](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |Lesen Sie die spezifischen Eigenschaften der eines der Objekte DirectorySettingTemplate System definiert.|
|[Liste directorySettingTemplate](../api/directorysettingtemplate-list.md) | [Auflistung von directorySettingTemplate](directorysettingtemplate.md) |Listen Sie aller vom System definierten DirectorySettingTemplate Objekte auf.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|description|string|Beschreibung der Vorlage. Schreibgeschützt.|
|displayName|string|Anzeigename der Vorlage. Schreibgeschützt. |
|id|string| Der eindeutige Bezeichner für die Vorlage. Schreibgeschützt.|
|values|[settingTemplateValue](settingtemplatevalue.md)-Sammlung| Sammlung von settingTemplateValues, die den Satz der verfügbaren Einstellungen, Standardwerte und Typen auflistet, die diese Vorlage bilden.  Schreibgeschützt. |

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
