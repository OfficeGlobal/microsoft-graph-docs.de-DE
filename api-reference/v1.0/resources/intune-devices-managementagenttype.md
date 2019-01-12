---
title: ManagementAgentType Enum-Typ
description: Typ der Management Agent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b76231a2781a153c5384c1dc3efdf8facec04dcc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966167"
---
# <a name="managementagenttype-enum-type"></a>ManagementAgentType Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Typ der Management Agent.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|EAS|1|Das Gerät wird vom Exchange-Server verwaltet.|
|MDM|2|Das Gerät wird durch Intune MDM verwaltet.|
|easMdm|3|Das Gerät wird von Exchange Server und Intune MDM verwaltet.|
|intuneClient|4|Intune Client verwaltet.|
|easIntuneClient|5|Das Gerät ist EAS Intune-Client und zwei verwaltet.|
|configurationManagerClient|8|Das Gerät wird vom Konfigurations-Manager verwaltet.|
|configurationManagerClientMdm|10|Das Gerät wird vom Konfigurations-Manager und MDM verwaltet.|
|configurationManagerClientMdmEas|11|Das Gerät wird vom Konfigurations-Manager, MDM und Eas verwaltet.|
|unknown|16|Unbekannte Management Agent-Typ.|
|jamf|32|Das Gerätattribute werden aus Jamf abgerufen.|
|googleCloudDevicePolicyController|64|Das Gerät wird von Google CloudDPC verwaltet.|



