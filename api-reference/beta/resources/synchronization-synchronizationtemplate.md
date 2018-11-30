---
title: Ressourcentyp SynchronisationVorlage
description: " Jeder Benutzer kann die Vorlage, um die Standardeinstellungen, einschließlich des Synchronisierungsschemas finden Sie unter abrufen."
ms.openlocfilehash: 90850ad43fdd14fc38ff6ae8cfa97f47806a289d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062232"
---
# <a name="synchronizationtemplate-resource-type"></a>Ressourcentyp SynchronisationVorlage

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Enthält vorkonfigurierte synchronisierungseinstellungen für eine bestimmte Anwendung. Standardmäßig werden diese Einstellungen für [Synchronisierungsauftrag](synchronization-synchronizationjob.md) verwendet, die auf der Vorlage basiert. Der Anwendungsentwickler gibt die Vorlage an. Jeder Benutzer kann die Vorlage, um die Standardeinstellungen, einschließlich der [Synchronisierungsschema](synchronization-synchronizationschema.md)finden Sie unter abrufen.

Sie können mehrere Vorlagen für eine Anwendung bereitstellen und eine entsprechende Standardvorlage bestimmen. Wenn mehrere Vorlagen für die Anwendung verfügbar, den, denen Sie interessiert sind sind, seek dienstanwendungsspezifische Anleitung, um zu bestimmen, welches am besten Ihren Anforderungen entspricht.

## <a name="methods"></a>Methoden

| Methode        | Rückgabetyp               | Beschreibung                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |[SynchronisationVorlage](synchronization-synchronizationtemplate.md) -Auflistung  |Listenvorlagen Sie für eine Anwendung oder Anwendungsinstanz (Service Principal) verfügbar sind.|
|[Get](../api/synchronization-synchronizationtemplate-get.md)      |[SynchronisationVorlage](synchronization-synchronizationtemplate.md)   |Lesen Sie die Eigenschaften und Beziehungen des **SynchronisationVorlage** -Objekts.|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ                      | Beschreibung                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |String                     |Eindeutige Vorlagenbezeichner.|
|applicationId  |Zeichenfolge                     |Bezeichner der Anwendung, zu der diese Vorlage gehört.|
|default        |Boolesch                    |`true`Wenn diese Vorlage als Standard für die Anwendung empfohlen wird.|
|description    |Zeichenfolge                     |Beschreibung der Vorlage.|
|eDiscovery-fähigen   |String                     |`true`Wenn diese Vorlage in der Auflistung der für die Instanz der Anwendung (Service Principal) verfügbaren Vorlagen angezeigt werden soll.|
|factoryTag     |String                     |Einer der bekannten Factory Tags durch das Synchronisierungsmodul unterstützt. Die **FactoryTag** weist dem Synchronisierungsmodul welche-Implementierung, bei der Verarbeitung von Aufträgen, die auf dieser Vorlage basierende.|
|Metadaten       |MetadataEntry-Auflistung   |Zusätzliche Erweiterungseigenschaften. Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.|

## <a name="relationships"></a>Beziehungen
| Beziehung      | Typ      |Beschreibung|
|:------------------|:----------|:----------|
|Schema             |[synchronizationSchema](synchronization-synchronizationschema.md)     |Synchronisierung-Standardschema für die auf dieser Vorlage basierende Aufträge.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->