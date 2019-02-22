---
title: firewallCertificateRevocationListCheckMethodType-Enumerationstyp
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74989961978ddd10f2c14e57cfe31e25ac831703
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170077"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType-Enumerationstyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte für firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts|
|Keine|1|Zertifikatsperrliste nicht überprüfen|
|Versuch|2|Versuchen Sie die Zertifikatsperrlistenüberprüfung und lassen Sie ein Zertifikat nur zu, wenn es von der Prüfung bestätigt wird.|
|erfordern|3|Erfolgreiche CRL-Überprüfung erfordern, bevor ein Zertifikat zugelassen wird|




