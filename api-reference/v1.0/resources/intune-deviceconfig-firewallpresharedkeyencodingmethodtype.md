---
title: firewallPreSharedKeyEncodingMethodType-Enumerationstyp
description: Mögliche Werte für firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c62144ef2974da5a3d975c759bb8d2bd2be6032
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259549"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a>firewallPreSharedKeyEncodingMethodType-Enumerationstyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte für firewallPreSharedKeyEncodingMethod

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|deviceDefault|0|Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts|
|Keine|1|Der vorinstallierte Schlüssel ist nicht codiert. Stattdessen wird es im Breitzeichen Format beibehalten.|
|utF8|2|Codieren des vorinstallierten Schlüssels mithilfe von UTF-8|



