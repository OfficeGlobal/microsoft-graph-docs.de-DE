---
title: Ressourcentyp „iosVppEBook“
description: Diese Klasse enthält die Eigenschaften eines iOS-VPP-E-Books.
author: tfitzmac
ms.openlocfilehash: a54c3a846be339dd1b7dcb98169e249122899d84
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362090"
---
# <a name="iosvppebook-resource-type"></a>Ressourcentyp „iosVppEBook“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|id|String|Schlüssel der Entität. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|displayName|String|Name des E-Books. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|description|String|Beschreibung. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|publisher|String|Herausgeber. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|publishedDateTime|DateTimeOffset|Datum und Uhrzeit der Veröffentlichung des E-Books. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Umschlagbild des Buchs. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der E-Book-Datei. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des E-Books. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|informationUrl|String|URL zur Seite mit weiteren Informationen. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|privacyInformationUrl|String|URL zur Datenschutzerklärung. Geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|vppTokenId|Guid|ID des VPP-Tokens|
|appleId|String|Apple-ID, die dem VPP-Token zugeordnet ist|
|vppOrganizationName|String|Zum VPP-Token gehörender Organisationsname|
|genres|Collection von Objekten des Typs „String“|Genres|
|language|String|Sprache|
|seller|String|Verkäufer|
|totalLicenseCount|Int32|Gesamtanzahl von Lizenzen|
|usedLicenseCount|Int32|Gesamtanzahl von genutzten Lizenzen|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung|Die Liste der Zuweisungen des E-Books. Der Wert wird geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Die Installationszusammenfassung für die mobile App. Der Wert wird geerbt von [managedEBook](../resources/intune-books-managedebook.md).|
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
  "usedLicenseCount": 1024
}
```



