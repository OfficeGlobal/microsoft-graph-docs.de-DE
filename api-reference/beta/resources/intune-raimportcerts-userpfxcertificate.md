---
title: userPFXCertificate-Ressourcentyp
description: Entity, die alle für die PFX-Zertifikate eines Benutzers erforderlichen Informationen kapselt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 534b2fa0f5f3240ead38deae45d3cc88091e40d8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154929"
---
# <a name="userpfxcertificate-resource-type"></a>userPFXCertificate-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Entity, die alle für die PFX-Zertifikate eines Benutzers erforderlichen Informationen kapselt.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Userpfxcertificateswurde aufListen](../api/intune-raimportcerts-userpfxcertificate-list.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekte.|
|[UserPFXCertificate abrufen](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Lesen von Eigenschaften und Beziehungen des [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.|
|[UserPFXCertificate erstellen](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Erstellen eines neuen [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.|
|[UserPFXCertificate löschen](../api/intune-raimportcerts-userpfxcertificate-delete.md)|Keine|Löscht eine [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).|
|[UserPFXCertificate aktualisieren](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Aktualisieren der Eigenschaften eines [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|string|Eindeutiger Bezeichner für das PFX-Zertifikat.|
|Fingerabdruck|Zeichenfolge|SHA-1 Fingerabdruck des PFX-Zertifikats.|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Zweck des Zertifikats aus der Sicht der Bereitstellung. Mögliche Werte: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|Zeichenfolge|Benutzerprinzipal Name des PFX-Zertifikats.|
|startDateTime|DateTimeOffset|Gültigkeitsdatum/-Uhrzeit des Zertifikats.|
|expirationDateTime|DateTimeOffset|Gültigkeitsablauf Datum/-Uhrzeit des Zertifikats.|
|providerName|Zeichenfolge|Crypto-Anbieter, der zum Verschlüsseln dieses BLOBs verwendet wird.|
|keyName|Zeichenfolge|Der Name des Schlüssels (innerhalb des Anbieters), der zum Verschlüsseln des BLOBs verwendet wird.|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Vom Anbieter während der Verschlüsselung/Entschlüsselung verwendetes Padding-Schema. Mögliche Werte sind: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384` und `oaepSha512`.|
|encryptedPfxBlob|Binär|Verschlüsselter PFX-BLOB.|
|encryptedPfxPassword|Zeichenfolge|Kennwort für verSchlüsselte PFX.|
|createdDateTime|DateTimeOffset|Datum/Uhrzeit des Imports dieses PFX-Zertifikats.|
|lastModifiedDateTime|DateTimeOffset|Datum/Uhrzeit der letzten Änderung dieses PFX-Zertifikats.|

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




