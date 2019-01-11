---
title: ManagementAgentType Enum-Typ
description: Typ der Management Agent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b8b4f5086ada7351dd41ac165dc600f81dc1fb4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813825"
---
# <a name="managementagenttype-enum-type"></a>ManagementAgentType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
|microsoft365ManagedMdm|258|Dieses Gerät wird von Microsoft 365 über Intune verwaltet.|





