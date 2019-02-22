---
title: managementAgentType-Enumerationstyp
description: Verwaltungs-Agenttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb948626035bed2dac7ee18d103aa083bd0f2aeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172541"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Verwaltungs-Agenttyp.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|EAS|1|Das Gerät wird von Exchange Server verwaltet.|
|MDM|2|Das Gerät wird von InTune MDM verwaltet.|
|easMdm|3|Das Gerät wird sowohl von Exchange Server als auch von InTune MDM verwaltet.|
|intuneClient|4|InTune-Client verwaltet.|
|easIntuneClient|5|Das Gerät ist EAS und InTune-Client Dual verwaltet.|
|configurationManagerClient|8|Das Gerät wird von Configuration Manager verwaltet.|
|configurationManagerClientMdm|10|Das Gerät wird von Configuration Manager und MDM verwaltet.|
|configurationManagerClientMdmEas|11|Das Gerät wird von Configuration Manager, MDM und EAS verwaltet.|
|unknown|16|UnBekannter Verwaltungs-Agenttyp.|
|JAMF|32|Die Geräteattribute werden aus JAMF abgerufen.|
|googleCloudDevicePolicyController|64|Das Gerät wird von Googles CloudDPC verwaltet.|
|microsoft365ManagedMdm|258|Dieses Gerät wird von Microsoft 365 über InTune verwaltet.|




