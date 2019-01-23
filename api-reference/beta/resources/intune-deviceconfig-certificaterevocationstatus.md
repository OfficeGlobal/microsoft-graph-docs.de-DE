---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 373cb6247a695a5912d02d4fb1a353c40aeac581
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421970"
---
# <a name="certificaterevocationstatus-enum-type"></a>CertificateRevocationStatus Enum-Typ

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Status der Zertifikatsperre.

## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|Nicht gesperrt.|
|Ausstehende|1|OCSP ausstehende.|
|ausgestellt|2|OCSP-Befehl ausgegeben.|
|failed|3|OCSP ist fehlgeschlagen.|
|widerrufen|4|Widerrufen.|




