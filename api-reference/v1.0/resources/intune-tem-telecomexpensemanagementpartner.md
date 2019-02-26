---
title: telecomExpenseManagementPartner-Ressourcentyp
description: TelecomExpenseManagementPartner-Ressourcen stellen die Metadaten und den Status eines bestimmten TEM-Diensts dar. Nach dem Ihre Organisation das Onboarding mit einem Partner abgeschlossen hat, kann für diesen das Ein-/Ausschalten der TEM-Funktionalität aktiviert oder deaktiviert werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d300fb881576932350eb60a6b441fa3087e6e5e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260193"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a>telecomExpenseManagementPartner-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|string|Eindeutiger Bezeichner des TEM-Partners|
|displayName|Zeichenfolge|Anzeigename des TEM-Partners|
|url|Zeichenfolge|Die URL für die Verwaltungssteuerung des TEM-Partners, mit der ein Administrator den TEM-Dienst konfigurieren kann.|
|appAuthorized|Boolean|Gibt an, ob die AAD-App des Partners für den Zugriff auf Intune autorisiert wurde.|
|enabled|Boolean|Gibt an, ob die Intune-Verbindung mit dem TEM-Dienst derzeit aktiviert oder deaktiviert ist.|
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



