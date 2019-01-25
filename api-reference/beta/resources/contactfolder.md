---
title: Ressourcentyp contactFolder
description: Ein Ordner, der Kontakte enthält.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 599f1765b6305d2dc4d482ec035ee4b24eb5183a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523799"
---
# <a name="contactfolder-resource-type"></a>Ressourcentyp contactFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ein Ordner, der Kontakte enthält.

Diese Ressource unterstützt die Verwendung einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen einer [delta](../api/contactfolder-delta.md)-Funktion.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[contactFolder abrufen](../api/contactfolder-get.md) | [contactFolder](contactfolder.md) |Dient zum Abrufen eines Kontaktordners anhand der Kontaktordner-ID.|
|[Aktualisieren](../api/contactfolder-update.md) | [contactFolder](contactfolder.md) |Dient zum Aktualisieren des contactFolder-Objekts. |
|[Löschen](../api/contactfolder-delete.md) | Keine |Dient zum Löschen des contactFolder-Objekts. |
|[childFolders auflisten](../api/contactfolder-list-childfolders.md) |[ContactFolder](contactfolder.md) collection| Dient zum Abrufen einer Sammlung von untergeordneten Ordnern unter dem angegebenen Kontaktordner.|
|[Untergeordneten contactFolder erstellen](../api/contactfolder-post-childfolders.md) |[contactFolder](contactfolder.md)| Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners.|
|[delta](../api/contact-delta.md)|[contact](contact.md)-Sammlung| Dient zum Abrufen eines Satzes von Kontaktordnern, die dem Postfach des Benutzers hinzugefügt bzw. daraus gelöscht oder entfernt wurden.|
|[Kontakte im Ordner auflisten](../api/contactfolder-list-contacts.md) |[contact](contact.md)-Sammlung| Dient zum Abrufen einer Kontaktsammlung aus dem Standardkontaktordner des angemeldeten Benutzers (`.../me/contacts`) oder aus dem angegebenen Kontaktordner.|
|[Kontakt in Ordner erstellen](../api/contactfolder-post-contacts.md) |[Kontakt](contact.md)| Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.|
|**Erweiterte Eigenschaften**| | |
|[Create single-value extended property](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[contactFolder](contactfolder.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.   |
|[contactFolder mit erweiterter einwertiger Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | Dient zum Abrufen von contactFolders-Elementen mit einer erweiterten einwertigen Eigenschaft mithilfe von `$expand` oder `$filter`. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [contactFolder](contactfolder.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen contactFolder-Element.  |
|[contactFolder mit erweiterter mehrwertiger Eigenschaft abrufen](../api/multivaluelegacyextendedproperty-get.md)  | [contactFolder](contactfolder.md) | Dient zum Abrufen eines contactFolders-Elements mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|displayName|Zeichenfolge|Der Anzeigename des Ordners.|
|id|String|Eindeutiger Bezeichner des Kontaktordners. Schreibgeschützt.|
|parentFolderId|Zeichenfolge|Die ID des übergeordneten Ordners des Ordners.|
|wellKnownName|string|Der Name des Ordners, wenn der Ordner einen erkannten Ordner ist. Derzeit `contacts` ist die einzige erkannten Kontakteordner.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|childFolders|[ContactFolder](contactfolder.md)-Sammlung|Die Sammlung der untergeordneten Ordner im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.|
|Kontakte|[Contact](contact.md)-Sammlung|Die Kontakte im Ordner. Navigationseigenschaft. Schreibgeschützt. Lässt NULL-Werte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter mehrwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter einwertiger Eigenschaften, die für das contactFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "contacts",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contactFolder"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "wellKnownName": "string"
}

```

## <a name="see-also"></a>Siehe auch

- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](/graph/delta-query-overview)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](/graph/delta-query-messages)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contactFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contactfolder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
