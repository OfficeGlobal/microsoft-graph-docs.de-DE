---
title: Ressourcentyp synchronizationSchema
description: Definiert, welche Objekte werden synchronisiert, und wie diese synchronisiert werden soll. Das Synchronisierungsschema enthält die meisten der Setupinformationen für einen bestimmten Synchronisierungsauftrag. Sie werden in der Regel anpassen einiger Attribut Zuordnungen oder Hinzufügen eines Gültigkeitsbereichs Filters zum Synchronisieren von nur Objekte, die eine bestimmte Bedingung erfüllen.
ms.openlocfilehash: 13e57db5f78af2d3f0a8243d247fe5c3f3d5e0af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061461"
---
# <a name="synchronizationschema-resource-type"></a>Ressourcentyp synchronizationSchema

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Definiert, welche Objekte werden synchronisiert, und wie diese synchronisiert werden soll. Das Synchronisierungsschema enthält die meisten der Setupinformationen für einen bestimmten Synchronisierungsauftrag. Sie werden in der Regel anpassen einiger [Attribut Zuordnungen](synchronization-attributemapping.md)oder Hinzufügen eines [Gültigkeitsbereichs Filter](synchronization-filter.md) , um nur die Objekte zu synchronisieren, die eine bestimmte Bedingung erfüllen.

In den folgenden Abschnitten werden die allgemeinen Komponenten des Synchronisierungsschemas beschrieben.

## <a name="directory-definitions"></a>Directory-Definitionen

[Directory-Definitionen](synchronization-directorydefinition.md) finden Sie die Synchronisierung Engine Verzeichnisse und deren Objekte Informationen. Die Definition Directory gibt beispielsweise dem Synchronisierungsmodul, dass ein Azure AD-Verzeichnis enthält Objekte, die mit der **Benutzer** und **Gruppen**, welche Attribute für diese Objekte und die Typen für diese Attribute unterstützt werden. In der Reihenfolge für ein bestimmtes Objekt und das Attribut im Synchronisierung Rules-Objekt Zuordnungen verwendet werden soll müssen sie als Teil der Definition der Directory definiert werden.

## <a name="synchronization-rules"></a>Synchronisierungsregeln

[Synchronisierungsregeln](synchronization-synchronizationrule.md) sind die Kernelemente der Synchronisation Einrichtung. Sie definieren für das Synchronisierungsmodul wie die Synchronisierung ausgeführt werden sollen, welche Objekte einschließlich synchronisiert werden soll, wie Objekte aus dem Quellverzeichnis-Objekte in das Zielverzeichnis zugeordnet werden soll, und wie Attribute werden sollen transformiert, wenn sie von der Quelle in das Zielverzeichnis synchronisiert sind. 

## <a name="object-mappings"></a>Objekt-Zuordnungen

[Objekt Zuordnungen](synchronization-objectmapping.md) sind die wichtigsten Teil der Regel Synchronisierung. Jede objektzuordnung definiert, wie ein bestimmtes Objekt aus der Quelle in das Zielverzeichnis synchronisiert werden sollen. Insbesondere die Zuordnung definiert, wie ein Objekt in das Quellverzeichnis mit einem Objekt in das Zielverzeichnis zugeordnet werden sollen was (falls vorhanden) Bereichsdefinierung Filter sollte verwendet werden, um festzulegen, ob ein Objekt bereit, und wie Objektattribute transformiert werden sollten Wenn sie von der Quelle in das Zielverzeichnis synchronisiert sind.

## <a name="methods"></a>Methoden

| Methode        | Rückgabetyp               | Beschreibung                  |
|:--------------|:--------------------------|:-----------------------------|
|[Get-schema](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |Lesen Sie Eigenschaften und Beziehungen des **SynchronizationSchema** -Objekts.|
|[Aktualisieren des Schemas](../api/synchronization-synchronizationschema-update.md)    |Keines   |Aktualisieren Sie das Synchronisierungsschema. |
|[Schema löschen](../api/synchronization-synchronizationschema-delete.md)    |Keines   |Löschen Sie das angepasste Schema, das Schema auf die Standardkonfiguration zurücksetzen. |
|[Liste Filteroperatoren](../api/synchronization-synchronizationschema-filteroperators.md)    |[FilterOperatorSchema](../resources/synchronization-filteroperatorschema.md) -Auflistung   |Alle in den Gültigkeitsbereichen Filtern unterstützte Operatoren aufgelistet. |
|[List-Attribut Zuordnen von Funktionen](../api/synchronization-synchronizationschema-functions.md)    |[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) -Auflistung   |Listen Sie alle Funktionen, die in das Attribut Zuordnung Ausdrücken unterstützt. |
|[Analysieren von Attribut Zuordnung Ausdruck](../api/synchronization-synchronizationschema-parseexpression.md)|[parseExpressionResponse](synchronization-parseexpressionresponse.md)|Ein Zeichenfolgenausdruck in einem [AttributeMappingSource analysieren|(.. / resources/synchronization_attributemappingsource.md) Objekt.|


## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ      | Beschreibung    |
|:--------------|:----------|:---------------|
|directories            |[DirectoryDefinition](synchronization-directorydefinition.md) -Auflistung   |Beschreibt Verzeichnisse und Objekte, die Teil der [SynchronizationJob](synchronization-synchronizationjob.md) oder [SynchronisationVorlage](synchronization-synchronizationtemplate.md)sind. |
|synchronizationRules   |[SynchronizationRule](synchronization-synchronizationrule.md) -Auflistung   |Eine Auflistung von Regeln für die [SynchronizationJob](synchronization-synchronizationjob.md) oder [SynchronisationVorlage](synchronization-synchronizationtemplate.md)konfiguriert sind, |
|Version                |String                             |Die Version des Schemas, bei jeder Änderung Schema automatisch aktualisiert.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchema"
}-->

```json
{
  "directories": [{"@odata.type": "microsoft.graph.directoryDefinition"}],
  "provisioningTaskIdentifier": "String (identifier)",
  "synchronizationRules": [{"@odata.type": "microsoft.graph.synchronizationRule"}],
  "version": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->