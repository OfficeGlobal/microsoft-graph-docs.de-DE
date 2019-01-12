---
title: Ressourcentyp userPFXCertificate
description: Entität, die kapselt alle Informationen für einen Benutzer PFX-Zertifikate erforderlich sind.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f63f95bb96e379cd2fcff0f0a50ac02162223ac2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987727"
---
# <a name="userpfxcertificate-resource-type"></a>Ressourcentyp userPFXCertificate

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Entität, die kapselt alle Informationen für einen Benutzer PFX-Zertifikate erforderlich sind.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste userPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|[UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Auflistung|Listeneigenschaften und Beziehungen der [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekte.|
|[Abrufen von userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Lesen Sie Eigenschaften und Beziehungen des [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.|
|[Erstellen von userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Erstellen eines neuen [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.|
|[UserPFXCertificate löschen](../api/intune-raimportcerts-userpfxcertificate-delete.md)|Keine|Löscht eine [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).|
|[UserPFXCertificate aktualisieren](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Aktualisieren Sie die Eigenschaften eines [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für das PFX-Zertifikat.|
|Fingerabdruck|Zeichenfolge|SHA-1-Fingerabdruck des Zertifikats PFX.|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Des Zertifikats beabsichtigten Zweck aus der Punkt der Ansicht der Bereitstellung. Mögliche Werte sind: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn` und `wifi`.|
|userPrincipalName|Zeichenfolge|Benutzerprinzipalname des PFX-Zertifikats.|
|startDateTime|DateTimeOffset|Gültigkeitsdauer der starten Datum/Uhrzeit.|
|expirationDateTime|DateTimeOffset|Des Zertifikats Gültigkeit Ablauf Datum/Uhrzeit.|
|providerName|Zeichenfolge|Kryptografieanbieter zum Verschlüsseln von diesem Blob verwendet.|
|Schlüsselname|Zeichenfolge|Name des Schlüssels (innerhalb der Anbieter) verwendet, um den Blob zu verschlüsseln.|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Abstand bei der Verschlüsselung/Entschlüsselung der vom Anbieter verwendete Schema. Mögliche Werte sind: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384` und `oaepSha512`.|
|encryptedPfxBlob|Binär|Blob für verschlüsselte PFX.|
|encryptedPfxPassword|Zeichenfolge|Verschlüsselte PFX-Kennwort ein.|
|createdDateTime|DateTimeOffset|Datum/Uhrzeit, wenn dieses PFX-Zertifikat importiert wurde.|
|lastModifiedDateTime|DateTimeOffset|Datum/Uhrzeit der letzten dieses PFX-Zertifikat Änderung.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





