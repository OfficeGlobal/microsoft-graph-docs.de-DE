---
title: WiFiSecurityType Enum-Typ
description: Wi-Fi-Sicherheitstypen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73724041c223d50d0030bf27b780d6b694792a16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422131"
---
# <a name="wifisecuritytype-enum-type"></a>WiFiSecurityType Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




