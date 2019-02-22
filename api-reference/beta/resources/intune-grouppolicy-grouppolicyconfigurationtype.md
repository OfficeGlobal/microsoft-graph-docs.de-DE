---
title: groupPolicyConfigurationType-Enumerationstyp
description: Gruppenrichtlinien-Konfigurationstyp
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0d3a0daa73fef30e5425e188958bdc54e61778d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164687"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>groupPolicyConfigurationType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Gruppenrichtlinien-Konfigurationstyp

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|Richtlinie|0|Der Richtlinientyp tätowiert den Wert nicht, was bedeutet, dass der Wert entfernt wird, sodass der ursprüngliche Konfigurationswert verwendet werden kann. Der Richtlinientyp überschreitet die Anwendungs Konfigurationseinstellung, sodass die Anwendung den Wert immer erkennt. Der Richtlinientyp verhindert, dass der Benutzer den Wert über die Benutzeroberfläche der Anwendung ändert.|
|preference|1|Der Einstellungstyp verwendet Tattoo als Wert, was bedeutet, dass der Wert nicht aus der Registrierung entfernt wird. Der Einstellungstyp überschreibt den Benutzer konfiguriert-Wert und behält nicht den vorherigen Wert bei. Der Einstellungstyp verhindert nicht, dass der Benutzer den Wert über die Benutzeroberfläche der Anwendung ändert.|




