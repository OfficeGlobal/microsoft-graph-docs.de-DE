---
title: termsAndConditionsAssignment-Ressourcentyp
description: C) Richtlinie zu einer bestimmten Gruppe. Benutzer in der Gruppe müssen die Nutzungsbedingungen annehmen, um Geräte in Intune registrieren zu lassen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75c9946cead03b2d7c0630c29a9b28c47ac1b269
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919806"
---
# <a name="termsandconditionsassignment-resource-type"></a>termsAndConditionsAssignment-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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





