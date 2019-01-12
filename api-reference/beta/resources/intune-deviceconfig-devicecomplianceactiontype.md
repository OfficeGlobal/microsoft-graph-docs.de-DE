---
title: DeviceComplianceActionType Enum-Typ
description: Geplante Aktion Typ Enum
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1856847cb8a8ecf48ee6d13067bd24515326d89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973209"
---
# <a name="devicecomplianceactiontype-enum-type"></a>DeviceComplianceActionType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Geplante Aktion Typ Enum
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|noAction|0|Keine Aktion|
|Benachrichtigung|1|Benachrichtigung senden|
|Blockieren|2|Das Gerät im AAD blockieren|
|Zurückziehen|3|Deaktivieren Sie das Gerät|
|Wischen|4|Bereinigen des Geräts|
|removeResourceAccessProfiles|5|Ressource Access Profile vom Gerät zu entfernen|
|pushNotification|9|Push-Benachrichtigung an Gerät senden|
|remoteLock|10|Das Gerät Remote Sperren|





