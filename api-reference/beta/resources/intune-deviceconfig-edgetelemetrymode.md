---
title: EdgeTelemetryMode Enum-Typ
description: Typ der Suchdaten an Microsoft 365 Analytics gesendet
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430092"
---
# <a name="edgetelemetrymode-enum-type"></a>EdgeTelemetryMode Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Typ der Suchdaten an Microsoft 365 Analytics gesendet

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|nicht konfiguriert|0|Standard – keine Telemetriedaten gesammelt oder gesendet|
|Intranet|1|Senden von Intranet Verlauf nur zugelassen: nur Organisations-Browser Verlaufsdaten für Intranetwebsites senden|
|internet|2|Senden von Internet-Verlauf nur zugelassen: nur senden durchsuchen Verlaufsdaten für Internetsites|
|intranetAndInternet|3|Senden von Intranet und Internet Verlauf zugelassen: Durchsuchen Verlaufsdaten für Intranet-und Internet senden|




