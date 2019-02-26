---
title: firewallCertificateRevocationListCheckMethodType-Enumerationstyp
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a475f32d4572b0aa8ed2a52befc7a58eb6077253
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257631"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a>firewallCertificateRevocationListCheckMethodType-Enumerationstyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte für firewallCertificateRevocationListCheckMethod

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts|
|Keine|1|Zertifikatsperrliste nicht überprüfen|
|Versuch|2|Versuchen Sie die Zertifikatsperrlistenüberprüfung und lassen Sie ein Zertifikat nur zu, wenn es von der Prüfung bestätigt wird.|
|erfordern|3|Erfolgreiche CRL-Überprüfung erfordern, bevor ein Zertifikat zugelassen wird|



