---
title: WiFiSecurityType Enum-Typ
description: Wi-Fi-Sicherheitstypen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6ddadaa31febaea08050ad49ffa540de53ff4819
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920219"
---
# <a name="wifisecuritytype-enum-type"></a>WiFiSecurityType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Wi-Fi-Sicherheitstypen.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|Öffnen Sie|0|Öffnen Sie (keine Authentifizierung).|
|wpaPersonal|1|WPA-Persönlich.|
|wpaEnterprise|2|WPA-Unternehmen. Muss einen IOSEnterpriseWifiConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.|
|WEP|3|WEP-Verschlüsselung.|
|wpa2Personal|4|WPA2-Persönlich.|
|wpa2Enterprise|5|WPA2-Unternehmen. Muss einen WindowsWifiEnterpriseEAPConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.|





