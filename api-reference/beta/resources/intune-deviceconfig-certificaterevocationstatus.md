---
title: CertificateRevocationStatus Enum-Typ
description: Status der Zertifikatsperre.
author: tfitzmac
ms.openlocfilehash: d41845ba882136c15d944c8a7f91083e6fa47cdb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358226"
---
# <a name="certificaterevocationstatus-enum-type"></a>CertificateRevocationStatus Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Status der Zertifikatsperre.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|Keine|0|Nicht gesperrt.|
|Ausstehende|1|OCSP ausstehende.|
|ausgestellt|2|OCSP-Befehl ausgegeben.|
|failed|3|OCSP ist fehlgeschlagen.|
|widerrufen|4|Widerrufen.|





