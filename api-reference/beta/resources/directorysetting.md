---
title: Verzeichnisberechtigungen Ressourcentyp
description: Directory-Einstellungen können basierend auf der verfügbaren DirectorySettingTemplates erstellt und Standardwerte voreingestellten von geändert werden. Diese Einstellungen können Entität oder ein Feature Verhaltensweisen, sowohl auf einem Mandanten-Ebene oder auf eine bestimmte Entitätsebene steuern. Wenn dieselbe Einstellung auf beide Mandanten geltende und bestimmte Entitätsebene definiert ist, die Einstellung der bestimmte Entität kann von der Einstellung für die gesamte Mandanten zielorientierten.  Beispielsweise die Einstellung für die gesamte Mandanten kann Gäste eingeladen werden, indem vorhandene Mitglieder von Gruppen, aber Einstellung für eine bestimmte Gruppe möglicherweise abmelden und nicht zulassen Gäste durch ein Mitglied der Gruppe eingeladen werden sollen. Derzeit definierten Systemeinstellungen sind nur Office Gruppen Verhalten steuern.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fbe1879a22b2dc7e69258d34f7e25c37bfd0cd5a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990551"
---
# <a name="directorysetting-resource-type"></a>Verzeichnisberechtigungen Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Directory-Einstellungen können basierend auf der verfügbaren [DirectorySettingTemplates](directorysettingtemplate.md)erstellt und die voreingestellte Standardeinstellung geändert werden. Diese Einstellungen können Entität oder ein Feature Verhaltensweisen, sowohl auf einem Mandanten-Ebene oder auf eine bestimmte Entitätsebene steuern. Wenn dieselbe Einstellung auf beide Mandanten geltende und bestimmte Entitätsebene definiert ist, die Einstellung der bestimmte Entität kann von der Einstellung für die gesamte Mandanten zielorientierten.  Beispielsweise die Einstellung für die gesamte Mandanten kann Gäste eingeladen werden, indem vorhandene Mitglieder von Gruppen, aber Einstellung für eine bestimmte Gruppe möglicherweise abmelden und nicht zulassen Gäste durch ein Mitglied der Gruppe eingeladen werden sollen. Derzeit definierten Systemeinstellungen sind nur Office Gruppen Verhalten steuern.

> **Hinweis**: die /beta Version von dem Ressourcentyp Verzeichnisberechtigungen gilt nur für Gruppen. Die Version /v1.0 wurde in GroupSetting umbenannt.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Einstellung erstellen](../api/directorysetting-post-settings.md) | [Verzeichnisberechtigungen](directorysetting.md) |Erstellen einer Einstellungsobjekt basierend auf einer DirectorySettingTemplate. Die POST-Anforderung muss EinstellenWerte für alle in der Vorlage definierten Einstellungen angeben.|
|[Einstellung abrufen](../api/directorysetting-get.md) | [Verzeichnisberechtigungen](directorysetting.md) |Dient zum Lesen der Eigenschaften eines bestimmten Einstellungsobjekts.|
|[Einstellungen auflisten](../api/directorysetting-list.md) | [Verzeichnisberechtigungen](directorysetting.md) -Auflistung |Listet Eigenschaften aller Einstellungsobjekte auf.|
|[Einstellung aktualisieren](../api/directorysetting-update.md) | [Verzeichnisberechtigungen](directorysetting.md)  |Aktualisiert ein Einstellungsobjekt. Nur EinstellenWerte können in einer Aktualisierung nicht geändert werden.|
|[Einstellung löschen](../api/directorysetting-delete.md) | Keine |Löscht ein Einstellungsobjekt. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|string|Anzeigename für diese Gruppe von Einstellungen, der aus der zugeordneten Vorlage stammt. Schreibgeschützt.|
|id|string| Eindeutiger Bezeichner für diese Einstellungen. Schreibgeschützt.|
|templateId|string| Eindeutiger Bezeichner für die Vorlage, die zum Erstellen dieser Gruppe von Einstellungen verwendet wird. Schreibgeschützt.|
|values|[settingValue](settingvalue.md)-Sammlung| Sammlung von Name/Wert-Paaren. Muss alle Einstellungen, die in dieser Vorlage definiert sind, enthalten und festlegen.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
