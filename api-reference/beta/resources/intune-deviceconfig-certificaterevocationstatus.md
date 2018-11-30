---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
ms.openlocfilehash: 5fb80b85cb6fe65e20439f8a3242b6bc74b30184
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059606"
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





