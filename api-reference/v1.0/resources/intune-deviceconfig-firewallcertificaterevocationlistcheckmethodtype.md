---
title: FirewallCertificateRevocationListCheckMethodType Enum-Typ
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e479b10339ab515a17f67d85de0c8d43c1507825
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940057"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>FirewallCertificateRevocationListCheckMethodType Enum-Typ

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für firewallCertificateRevocationListCheckMethod
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät|
|n/v|1|Zertifikatsperrliste nicht prüfen|
|Versuchen Sie|2|Versuchen Sie Zertifikatsperrlistenprüfung und zulassen Sie ein Zertifikat nur, wenn das Zertifikat mithilfe der Kontrollkästchen bestätigt wird|
|erfordern|3|Erfordern Sie eine erfolgreiche Zertifikatsperrlistenprüfung, bevor Sie ein Zertifikat|



