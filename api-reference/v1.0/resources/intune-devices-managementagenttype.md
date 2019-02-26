---
title: managementAgentType-Enumerationstyp
description: Verwaltungs-Agenttyp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9743c9c83e34a0c58dee78e73839f8fdcaaf2cda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251566"
---
# <a name="managementagenttype-enum-type"></a>managementAgentType-Enumerationstyp

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



