---
title: auditEvent-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für das Audit-Ereignis enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fd9971b5b6ddce9b3a826ff569d1925ef9cff97
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153676"
---
# <a name="auditevent-resource-type"></a>auditEvent-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine Klasse, die die Eigenschaften für das Audit-Ereignis enthält.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[auditEvents auflisten](../api/intune-auditing-auditevent-list.md)|[auditEvent](../resources/intune-auditing-auditevent.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [auditEvent](../resources/intune-auditing-auditevent.md)-Objekte.|
|[auditEvent abrufen](../api/intune-auditing-auditevent-get.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Lesen von Eigenschaften und Beziehungen des [auditEvent](../resources/intune-auditing-auditevent.md)-Objekts.|
|[auditEvent erstellen](../api/intune-auditing-auditevent-create.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Erstellen eines neuen [auditEvent](../resources/intune-auditing-auditevent.md)-Objekts.|
|[auditEvent löschen](../api/intune-auditing-auditevent-delete.md)|Keine|Löscht ein [auditEvent](../resources/intune-auditing-auditevent.md)-Objekt.|
|[auditEvent aktualisieren](../api/intune-auditing-auditevent-update.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Aktualisieren der Eigenschaften eines [auditEvent](../resources/intune-auditing-auditevent.md)-Objekts.|
|[getAuditCategories-Funktion](../api/intune-auditing-auditevent-getauditcategories.md)|Zeichenfolgenauflistung|Noch nicht dokumentiert|
|[getAuditActivityTypes-Funktion](../api/intune-auditing-auditevent-getauditactivitytypes.md)|String-Sammlung|Noch nicht dokumentiert.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|displayName|Zeichenfolge|Anzeigename des Ereignisses|
|componentName|Zeichenfolge|Name der Komponente|
|actor|[auditActor](../resources/intune-auditing-auditactor.md)|AAD-Benutzer und -Anwendung, die dem Überwachungsereignis zugeordnet sind|
|activity|Zeichenfolge|Anzeigename der Aktivität|
|activityDateTime|DateTimeOffset|Datum und Uhrzeit der Durchführung der Aktivität im UTC-Format|
|activityType|Zeichenfolge|Typ der durchgeführten Aktivität|
|activityOperationType|Zeichenfolge|HTTP-Vorgangstyp der Aktivität|
|activityResult|Zeichenfolge|Ergebnis der Aktivität|
|correlationId|Guid|ID der Clientanforderung, die zur Korrelation von Aktivitäten im System verwendet wird|
|resources|Collection von Objekten des Typs [auditResource](../resources/intune-auditing-auditresource.md)|Ressourcen, die geändert werden|
|category|String|Audit-Kategorie|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```




