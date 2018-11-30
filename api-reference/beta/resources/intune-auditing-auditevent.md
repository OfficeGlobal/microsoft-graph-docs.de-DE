---
title: auditEvent-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für das Audit-Ereignis enthält.
ms.openlocfilehash: 1846677ea72dda836f92e0d45d76ea0df0ae74f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064692"
---
# <a name="auditevent-resource-type"></a>auditEvent-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

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
|id|String|Schlüssel der Entität|
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





