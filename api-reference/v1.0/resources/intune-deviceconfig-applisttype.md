---
title: appListType-Enumerationstyp
description: Mögliche Werte der Kompatibilitäts-App-Liste.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 379ec2e10e68d62353875cd2b49c0944fe11f4da
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254324"
---
# <a name="applisttype-enum-type"></a>appListType-Enumerationstyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Mögliche Werte der Kompatibilitäts-App-Liste.

## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|Standardwert, keine Absicht.|
|appsInListCompliant|1|Die Liste stellt die apps dar, die als kompatibel betrachtet werden (nur apps in der Liste sind kompatibel).|
|appsNotInListCompliant|2|Die Liste stellt die apps dar, die als nicht kompatibel gelten (alle apps sind mit Ausnahme von apps in der Liste kompatibel).|



