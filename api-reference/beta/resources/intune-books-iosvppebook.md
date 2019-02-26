---
title: Ressourcentyp „iosVppEBook“
description: Diese Klasse enthält die Eigenschaften eines iOS-VPP-E-Books.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca890a6b15ac232d8fb685913379ba8bf69f35cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149441"
---
# <a name="iosvppebook-resource-type"></a>Ressourcentyp „iosVppEBook“

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Klasse enthält die Eigenschaften eines iOS-VPP-E-Books.


Sie erbt von [managedEBook](../resources/intune-books-managedebook.md).

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Auflisten von „iosVppEBook“](../api/intune-books-iosvppebook-list.md)|Sammlung von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md)|Listet die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md) auf.|
|[Abrufen von „iosVppEBook“](../api/intune-books-iosvppebook-get.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|Liest die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Erstellen von „iosVppEBook“](../api/intune-books-iosvppebook-create.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|Erstellt neue Objekte des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Löschen von „iosVppEBook“](../api/intune-books-iosvppebook-delete.md)|Keiner|Löscht Objekte des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Aktualisieren von „iosVppEBook“](../api/intune-books-iosvppebook-update.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|Aktualisiert die Eigenschaften von Objekten des Typs [iosVppEBook](../resources/intune-books-iosvppebook.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Schlüssel der Entität. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|displayName|Zeichenfolge|Name des E-Books. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|description|String|Beschreibung. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|publisher|Zeichenfolge|Herausgeber. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|publishedDateTime|DateTimeOffset|Datum und Uhrzeit der Veröffentlichung des E-Books. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Umschlagbild des Buchs. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der E-Book-Datei. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des E-Books. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|privacyInformationUrl|Zeichenfolge|URL zur Datenschutzerklärung. Der Wert wird geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|vppTokenId|Guid|ID des VPP-Tokens|
|appleId|Zeichenfolge|Apple-ID, die dem VPP-Token zugeordnet ist|
|vppOrganizationName|Zeichenfolge|Zum VPP-Token gehörender Organisationsname|
|genres|String collection|Genres|
|language|Zeichenfolge|Sprache|
|seller|Zeichenfolge|Verkäufer|
|totalLicenseCount|Int32|Gesamtanzahl von Lizenzen|
|usedLicenseCount|Int32|Gesamtanzahl von genutzten Lizenzen|
|Rolescopetagids zur|String collection|Liste der Bereichs Tags für diese Entitätsinstanz.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|[managedEBookCategory](../resources/intune-books-managedebookcategory.md) -Sammlung|Die Liste der Kategorien für dieses eBook. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|assignments|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung|Die Liste der Zuweisungen des E-Books. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|deviceStates|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung|Die Liste der Installationsstatus für das E-Book. Der Wert wird geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|userStateSummary|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Sammlung|Die Liste der Installationsstatus für das E-Book. Der Wert wird geerbt von [managedEBook](../resources/intune-books-managedebook.md).|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String",
  "vppTokenId": "Guid",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024,
  "roleScopeTagIds": [
    "String"
  ]
}
```




