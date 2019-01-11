---
title: WiFiSecurityType Enum-Typ
description: Wi-Fi-Sicherheitstypen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 90290b9b47154b95aca81d931fa66e7984688db1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839921"
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





