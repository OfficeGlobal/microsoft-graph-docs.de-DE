---
title: Ressourcentyp contact
description: Ein Kontakt ist ein Element in Outlook, in dem Sie Informationen über die Personen und Organisationen, mit denen Sie kommunizieren, organisieren und speichern können. Kontakte sind in Kontaktordnern enthalten.
ms.openlocfilehash: 1f18118855417727a441b25c008cee9a0e826aff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060711"
---
# <a name="contact-resource-type"></a>Ressourcentyp contact

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Kontakt ist ein Element in Outlook, in dem Sie Informationen über die Personen und Organisationen, mit denen Sie kommunizieren, organisieren und speichern können. Kontakte sind in Kontaktordnern enthalten.

Diese Ressource unterstützt Folgendes:

- Hinzufügen von Ihren eigenen Daten zu benutzerdefinierten Eigenschaften als [Extensions](/graph/extensibility-overview).
- Abonnieren von [Benachrichtigungen zu ändern](/graph/webhooks).
- Verwenden einer [Delta-Abfrage](/graph/delta-query-overview) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/contact-delta.md)-Funktion.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.typedEmailAddress"}],
  "fileAs": "string",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "gender": "string",
  "generation": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "nickName": "string",
  "officeLocation": "string",
  "parentFolderId": "string",
  "personalNotes": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.physicalAddress"}],
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "weddingAnniversary": "date",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assistantName|String|Der Name des Assistenten des Kontakts.|
|birthday|DateTimeOffset|Das Geburtsdatum des Kontakts. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|categories|Zeichenfolgenauflistung|Die Kategorien, die mit dem Kontakt verknüpft sind. Jeder Kategorie entspricht die **DisplayName** -Eigenschaft des ein [OutlookCategory](outlookcategory.md) für den Benutzer definiert.|
|changeKey|String|Gibt die Version des Kontakts an. Jedes Mal, wenn der Kontakt geändert wird, wird auch die Eigenschaft „changeKey“ geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.|
|children|Zeichenfolgenauflistung|Die Namen der Kinder des Kontakts.|
|companyName|String|Der Name des Unternehmens des Kontakts.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der Kontakt erstellt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Abteilung|String|Die Abteilung des Kontakts.|
|displayName|String|Der Anzeigename des Kontakts. Sie können den Anzeigenamen in einem Vorgang [Erstellen](../api/user-post-contacts.md) oder [Aktualisieren](../api/contact-update.md) angeben. Beachten Sie, dass es sich bei spätere Aktualisierungen mit anderen Eigenschaften verursachen einen automatisch generierten Wert den Wert DisplayName überschrieben, den Sie angegeben haben. Um einen bereits vorhandenen Wert zu erhalten, immer als schließen Sie DisplayName in einem Vorgang [zu aktualisieren ein](../api/contact-update.md) .|
|emailAddresses|[TypedEmailAddress](typedemailaddress.md) -Auflistung|Die E-Mail-Adressen des Kontakts.|
|fileAs|String|Der Name, unter dem der Kontakt abgelegt ist.|
|Flag|[followupFlag](followupflag.md)|Das Flagwert, der den Status, Startdatum, Fälligkeitsdatum oder Fertigstellungstermin für den Kontakt angibt. |
|gender |String |Geschlecht des Kontakts. |
|generation|String|Die Generation des Kontakts.|
|givenName|String|Der Vorname des Kontakts.|
|id|String|Eindeutiger Bezeichner für den Kontakt. Schreibgeschützt.|
|imAddresses|Zeichenfolgenauflistung|Instant Messaging Chatadressen des Kontakts.|
|initials|String|Die Initialen des Kontakts.|
|jobTitle|String|Die Position des Kontakts.|
|lastModifiedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der Kontakt geändert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|manager|String|Der Name des Vorgesetzten des Kontakts.
|middleName|String|Der zweite Vorname des Kontakts.|
|nickName|String|Der Spitzname des Kontakts.|
|officeLocation|String|Der Bürostandort des Kontakts.|
|parentFolderId|String|Die ID des übergeordneten Ordners des Kontakts.|
|personalNotes|String|Die Notizen des Benutzers zu dem Kontakt.|
|phones |[phone](phone.md)-Sammlung |Telefonnummern für den Kontakt zugeordnet ist, beispielsweise Telefon (privat), Mobiltelefon und Telefon (geschäftlich) |
|postalAddresses |[physikalische Adresse](physicaladdress.md) -Auflistung |Der Kontakt zugeordnete Adressen home beispielsweise Adresse und Geschäftsadresse. |
|profession|String|Der Beruf des Kontakts.|
|spouseName|Zeichenfolge|Der Name des Ehepartners/Partners des Kontakts|
|surname|String|Der Nachname des Kontakts.|
|title|String|Der Titel des Kontakts.|
|websites |[website](website.md)-Sammlung|Websites, die dem Kontakt zugeordnet werden. |
|weddingAnniversary |Datum |Hochzeitstag des Kontakts. |
|yomiCompanyName|String|Der phonetische japanische Firmenname des Kontakts.|
|yomiGivenName|String|Der phonetische japanische Vorname des Kontakts.|
|yomiSurname|String|Der phonetische japanische Nachname des Kontakts.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Auflistung der open-Erweiterungen für den Kontakt definiert. Lässt Nullwerte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter mehrwertiger Eigenschaften, die für den Kontakt definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|
|Foto|[photo](profilephoto.md)| Optionales Kontaktbild. Sie können für einen Kontakt ein Foto abrufen oder einstellen.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung erweiterter einwertiger Eigenschaften, die für den Kontakt definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|

## <a name="methods"></a>Methoden
| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Kontakt abrufen](../api/contact-get.md) | [Kontakt](contact.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des Kontaktobjekts.|
|[Erstellen](../api/user-post-contacts.md) | [Kontakt](contact.md) |Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Kontaktendpunkt eines anderen Kontaktordners.|
|[Aktualisieren](../api/contact-update.md) | [Kontakt](contact.md) |Dient zum Aktualisieren des Kontaktobjekts. |
|[Löschen](../api/contact-delete.md) | Keine |Dient zum Löschen des Kontaktobjekts. |
|[delta](../api/contact-delta.md)|[contact](contact.md)-Sammlung| Dient zum Abrufen eines Satzes von Kontakten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[Kontakt](contact.md)  |Dient zum Erstellen einer oder mehrerer erweiterter einwertiger Eigenschaften in einem neuen oder vorhandenen Kontakt.   |
|[Ereignis mit erweiterter einwertiger Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty-get.md)  | [Kontakt](contact.md) | Ruft mithilfe von `$expand` oder `$filter` Kontakte mit einer bestimmten einwertigen erweiterten Eigenschaft ab. |
|[Erweiterte mehrwertige Eigenschaft erstellen](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [Kontakt](contact.md) | Dient zum Erstellen einer oder mehrerer erweiterter mehrwertiger Eigenschaften in einem neuen oder vorhandenen Kontakt.  |
|[Ereignis mit erweiterter mehrwertiger Eigenschaft abrufen](../api/multivaluelegacyextendedproperty-get.md)  | [Kontakt](contact.md) | Dient zum Abrufen eines Kontakts mit einer erweiterten mehrwertigen Eigenschaft mithilfe von `$expand`. |

## <a name="see-also"></a>Siehe auch

- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](/graph/delta-query-overview)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](/graph/delta-query-messages)
- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
