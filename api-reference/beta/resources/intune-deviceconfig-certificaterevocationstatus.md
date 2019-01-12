---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c1c77e267da5528088a7a8ef6400a872790aaf3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983121"
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





