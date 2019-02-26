---
title: managedEBook-Ressourcentyp
description: Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6151c23bf05b076ade441f908a2810c80f45ed
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253463"
---
# <a name="managedebook-resource-type"></a>managedEBook-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|string|Schlüssel der Entität|
|displayName|Zeichenfolge|Name des E-Books|
|description|String|Beschreibung|
|publisher|String|Herausgeber|
|publishedDateTime|DateTimeOffset|Datum und Uhrzeit der Veröffentlichung des E-Books.|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Umschlagbild des Buchs|
|createdDateTime|DateTimeOffset|Datum und Uhrzeit der Erstellung der E-Book-Datei.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des E-Books.|
|informationUrl|Zeichenfolge|URL zur Seite mit weiteren Informationen.|
|privacyInformationUrl|Zeichenfolge|URL zur Datenschutzerklärung|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
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



