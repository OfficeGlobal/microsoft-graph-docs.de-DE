---
title: managedEBook-Ressourcentyp
description: Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
author: tfitzmac
ms.openlocfilehash: 7b826d7b0a11ce957a87154f276abc0e8168f45d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347145"
---
# <a name="managedebook-resource-type"></a>managedEBook-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedEBooks auflisten](../api/intune-books-managedebook-list.md)|[managedEBook](../resources/intune-books-managedebook.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedEBook](../resources/intune-books-managedebook.md)-Objekte.|
|[managedEBook abrufen](../api/intune-books-managedebook-get.md)|[managedEBook](../resources/intune-books-managedebook.md)|Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune-books-managedebook.md)-Objekts.|
|[Aktion zuweisen](../api/intune-books-managedebook-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|displayName|String|Name des E-Books|
|description|String|Beschreibung|
|publisher|String|Herausgeber|
|publishedDateTime|DateTimeOffset|Datum und Uhrzeit der Veröffentlichung des E-Books.|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Umschlagbild des Buchs|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der E-Book-Datei.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des E-Books.|
|informationUrl|String|URL zur Seite mit weiteren Informationen.|
|privacyInformationUrl|String|URL zur Datenschutzerklärung|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|categories|[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Auflistung|Die Liste der Kategorien für e-Book.|
|assignments|[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung|Die Liste der Zuweisungen für dieses E-Book.|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Die Installationszusammenfassung für die mobile App.|
|deviceStates|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung|Die Liste der Installationsstatus für das E-Book.|
|userStateSummary|[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Sammlung|Die Liste der Installationsstatus für das E-Book.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
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
  "privacyInformationUrl": "String"
}
```





