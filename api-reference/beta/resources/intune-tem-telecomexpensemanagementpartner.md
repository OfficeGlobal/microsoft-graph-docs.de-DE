---
title: telecomExpenseManagementPartner-Ressourcentyp
description: TelecomExpenseManagementPartner-Ressourcen stellen die Metadaten und den Status eines bestimmten TEM-Diensts dar. Nach dem Ihre Organisation das Onboarding mit einem Partner abgeschlossen hat, kann für diesen das Ein-/Ausschalten der TEM-Funktionalität aktiviert oder deaktiviert werden.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f6bbb76a98e664f759f8e543eecafe2df6167515
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923019"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a>telecomExpenseManagementPartner-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

TelecomExpenseManagementPartner-Ressourcen stellen die Metadaten und den Status eines bestimmten TEM-Diensts dar. Nach dem Ihre Organisation das Onboarding mit einem Partner abgeschlossen hat, kann für diesen das Ein-/Ausschalten der TEM-Funktionalität aktiviert oder deaktiviert werden.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[TelecomExpenseManagementPartners auflisten](../api/intune-tem-telecomexpensemanagementpartner-list.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekte.|
|[TelecomExpenseManagementPartner abrufen](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Lesen von Eigenschaften und Beziehungen des [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts.|
|[TelecomExpenseManagementPartner erstellen](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Erstellen eines neuen [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts.|
|[TelecomExpenseManagementPartner löschen](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|Keine|Löscht ein [TelecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekt.|
|[TelecomExpenseManagementPartner aktualisieren](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)|Aktualisieren der Eigenschaften eines [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner des TEM-Partners|
|displayName|Zeichenfolge|Anzeigename des TEM-Partners|
|url|Zeichenfolge|Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.|
|appAuthorized|Boolescher Wert|Gibt an, ob die AAD-App des Partners für den Zugriff auf Intune autorisiert wurde.|
|enabled|Boolescher Wert|Gibt an, ob die Intune-Verbindung mit dem TEM-Dienst derzeit aktiviert oder deaktiviert ist.|
|lastConnectionDateTime|DateTimeOffset|Zeitstempel der letzten vom TEM-Partner an Intune gesendeten Anforderung|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```





