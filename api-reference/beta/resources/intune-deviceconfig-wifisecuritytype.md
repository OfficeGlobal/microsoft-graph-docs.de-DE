---
title: WiFiSecurityType Enum-Typ
description: Wi-Fi-Sicherheitstypen.
author: tfitzmac
ms.openlocfilehash: 291bc3660971a90ea113959368542e715a86b570
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329190"
---
# <a name="wifisecuritytype-enum-type"></a>WiFiSecurityType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Wi-Fi-Sicherheitstypen.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|Öffnen Sie|0|Öffnen Sie (keine Authentifizierung).|
|wpaPersonal|1|WPA-Persönlich.|
|wpaEnterprise|2|WPA-Unternehmen. Muss einen IOSEnterpriseWifiConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.|
|WEP|3|WEP-Verschlüsselung.|
|wpa2Personal|4|WPA2-Persönlich.|
|wpa2Enterprise|5|WPA2-Unternehmen. Muss einen WindowsWifiEnterpriseEAPConfiguration-Typ verwenden, um Enterprise-Optionen zu konfigurieren.|





