---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d24d515f992ed396c3530595240a107852d83e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868306"
---
# <a name="certificaterevocationstatus-enum-type"></a>CertificateRevocationStatus Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Status der Zertifikatsperre.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|n/v|0|Nicht gesperrt.|
|Ausstehende|1|OCSP ausstehende.|
|ausgestellt|2|OCSP-Befehl ausgegeben.|
|failed|3|OCSP ist fehlgeschlagen.|
|widerrufen|4|Widerrufen.|





