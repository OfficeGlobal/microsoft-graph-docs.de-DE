---
title: ManagementAgentType Enum-Typ
description: Typ der Management Agent.
author: tfitzmac
ms.openlocfilehash: 702f71f3984bda34e31d0a614e45e387f45b587e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321588"
---
# <a name="managementagenttype-enum-type"></a>ManagementAgentType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Typ der Management Agent.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
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
|microsoft365ManagedMdm|258|Dieses Gerät wird von Microsoft 365 über Intune verwaltet.|





