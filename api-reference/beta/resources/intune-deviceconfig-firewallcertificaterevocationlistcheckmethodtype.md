---
title: FirewallCertificateRevocationListCheckMethodType Enum-Typ
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
ms.openlocfilehash: 302037187addfb8606c6c1e60a9369eb1f7c2ed5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320713"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>FirewallCertificateRevocationListCheckMethodType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Mögliche Werte für firewallCertificateRevocationListCheckMethod
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät|
|Keine|1|Zertifikatsperrliste nicht prüfen|
|Versuchen Sie|2|Versuchen Sie Zertifikatsperrlistenprüfung und zulassen Sie ein Zertifikat nur, wenn das Zertifikat mithilfe der Kontrollkästchen bestätigt wird|
|erfordern|3|Erfordern Sie eine erfolgreiche Zertifikatsperrlistenprüfung, bevor Sie ein Zertifikat|





