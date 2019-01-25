---
title: 'EducationSynchronizationProfile: UploadUrl'
description: Abrufen einer gemeinsamen Zugriff Signatur (SAS) für das Hochladen von Quelldateien in Azure Blob-Speicher für ein bestimmtes Schule Synchronisierung Datenprofil im Mandanten. Das Token SAS hat eine Gültigkeit von einer Stunde.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 74f37f5653147691c408cf83e3039920957352c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511597"
---
# <a name="educationsynchronizationprofile-uploadurl"></a>EducationSynchronizationProfile: UploadUrl

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abrufen einer gemeinsamen Zugriff Signatur (SAS) für das Hochladen von Quelldateien in Azure Blob-Speicher für eine bestimmte Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten. Das Token SAS hat eine Gültigkeit von einer Stunde.

Der Upload wird nur für die [CSV-Datenanbieter](../resources/educationcsvdataprovider.md)URL bereitgestellt.

> **Hinweis:** Verwenden Sie den Zugriff auf die Blob-Speicherung mit dem SAS-Token der [Azure-Speicher SDKs](https://github.com/search?q=org%3AAzure+azure-storage) oder [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp | Berechtigungen |
|:-----------|:----------|
| Delegiert (Geschäfts-, Schul- oder Unikonto) | EduAdministration.ReadWrite |
|Delegiert (persönliches Microsoft-Konto)|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine SAS-URL für die [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md) im Antworttext.

Wenn weiterhin eine vorherige Anforderung verarbeitet wird, gibt diese Methode einen `409 Conflict` zurück, der angibt, dass der Upload gegenwärtig für die [EducationSynchronizationProfile](../resources/educationsynchronizationprofile.md)ausgeschlossen wird.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
