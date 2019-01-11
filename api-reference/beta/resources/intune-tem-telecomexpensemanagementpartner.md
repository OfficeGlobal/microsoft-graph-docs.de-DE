---
title: telecomExpenseManagementPartner-Ressourcentyp
description: TelecomExpenseManagementPartner-Ressourcen stellen die Metadaten und den Status eines bestimmten TEM-Diensts dar. Nach dem Ihre Organisation das Onboarding mit einem Partner abgeschlossen hat, kann für diesen das Ein-/Ausschalten der TEM-Funktionalität aktiviert oder deaktiviert werden.
localization_priority: Normal
ms.openlocfilehash: 5fdc80b67c92fb7e47a38fd57d3a52db3459763a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825298"
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
|id|String|Eindeutiger Bezeichner des TEM-Partners|
|displayName|Zeichenfolge|Anzeigename des TEM-Partners|
|url|String|Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.|
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





