---
title: auditEvent-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für das Audit-Ereignis enthält.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3eddfcbd94153bfc1f7d1798f8806fb84b6341bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425162"
---
# <a name="auditevent-resource-type"></a>auditEvent-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Eine Klasse, die die Eigenschaften für das Audit-Ereignis enthält.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[auditEvents auflisten](../api/intune-auditing-auditevent-list.md)|[auditEvent](../resources/intune-auditing-auditevent.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [auditEvent](../resources/intune-auditing-auditevent.md)-Objekte.|
|[auditEvent abrufen](../api/intune-auditing-auditevent-get.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Lesen von Eigenschaften und Beziehungen des [auditEvent](../resources/intune-auditing-auditevent.md)-Objekts.|
|[auditEvent erstellen](../api/intune-auditing-auditevent-create.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Erstellen eines neuen [auditEvent](../resources/intune-auditing-auditevent.md)-Objekts.|
|[auditEvent löschen](../api/intune-auditing-auditevent-delete.md)|Keine|Löscht ein [auditEvent](../resources/intune-auditing-auditevent.md)-Objekt.|
|[auditEvent aktualisieren](../api/intune-auditing-auditevent-update.md)|[auditEvent](../resources/intune-auditing-auditevent.md)|Aktualisieren der Eigenschaften eines [auditEvent](../resources/intune-auditing-auditevent.md)-Objekts.|
|[getAuditCategories-Funktion](../api/intune-auditing-auditevent-getauditcategories.md)|String-Sammlung|Noch nicht dokumentiert|
|[getAuditActivityTypes-Funktion](../api/intune-auditing-auditevent-getauditactivitytypes.md)|String-Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|displayName|String|Anzeigename des Ereignisses|
|componentName|String|Name der Komponente|
|actor|[auditActor](../resources/intune-auditing-auditactor.md)|AAD-Benutzer und -Anwendung, die dem Überwachungsereignis zugeordnet sind|
|activity|String|Anzeigename der Aktivität|
|activityDateTime|DateTimeOffset|Datum und Uhrzeit der Durchführung der Aktivität im UTC-Format|
|activityType|String|Typ der durchgeführten Aktivität|
|activityOperationType|String|HTTP-Vorgangstyp der Aktivität|
|activityResult|String|Ergebnis der Aktivität|
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




