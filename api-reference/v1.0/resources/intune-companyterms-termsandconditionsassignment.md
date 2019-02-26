---
title: termsAndConditionsAssignment-Ressourcentyp
description: Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e4c8b7ac86f86f2b89bcd21a0576f68b823b9f6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262202"
---
# <a name="termsandconditionsassignment-resource-type"></a>termsAndConditionsAssignment-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine TermsAndConditionsAssignment-Entität steht für die Zuweisung einer bestimmten Richtlinie der Nutzungsbedingungen (Terms and Conditions, T&C) zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[termsAndConditionsAssignments auflisten](../api/intune-companyterms-termsandconditionsassignment-list.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekte.|
|[termsAndConditionsAssignment abrufen](../api/intune-companyterms-termsandconditionsassignment-get.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.|
|[termsAndConditionsAssignment erstellen](../api/intune-companyterms-termsandconditionsassignment-create.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Erstellen eines neuen [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.|
|[termsAndConditionsAssignment löschen](../api/intune-companyterms-termsandconditionsassignment-delete.md)|Keine|Löscht ein [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|
|[termsAndConditionsAssignment aktualisieren](../api/intune-companyterms-termsandconditionsassignment-update.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Aktualisieren der Eigenschaften eines [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner der Entität|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Zuweisungsziel, dem die Richtlinie der Nutzungsbedingungen zugewiesen wird.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



