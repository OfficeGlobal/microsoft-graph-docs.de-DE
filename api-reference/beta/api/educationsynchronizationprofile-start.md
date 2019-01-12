---
title: Nach dem Hochladen von Dateien in einer EducationSynchronizationProfile starten Sie Synchronisierung
description: Überprüfen Sie die Dateien auf einem bestimmten Schule Daten Synchronisierung Profil in den Mandanten hochgeladen. Wenn die Überprüfung erfolgreich ist, wird auf das Profil Synchronisierung starten. Andernfalls enthält die Antwort Fehler und Warnungen. Wenn die Antwort Fehler enthält, wird die Synchronisierung nicht gestartet. Wenn die Antwort nur Warnungen enthält, wird Synchronisierung starten.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: efdc0863a1de58f7ebf46492b662e632972275c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915249"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a>Nach dem Hochladen von Dateien in einer EducationSynchronizationProfile starten Sie Synchronisierung

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Überprüfen Sie die Dateien auf einem bestimmten Schule Daten [Synchronisierung Profil](../resources/educationsynchronizationprofile.md) im Mandanten hochgeladen. Wenn die Überprüfung erfolgreich ist, wird auf das Profil Synchronisierung starten. Andernfalls enthält die Antwort Fehler und Warnungen. Wenn die Antwort Fehler enthält, wird die Synchronisierung nicht gestartet. Wenn die Antwort nur Warnungen enthält, wird Synchronisierung starten.

> **Hinweis:** Verwenden Sie diese Methode nur, wenn Sie der Datenanbieter vom Typ [Educationcsvdataprovider](../resources/educationcsvdataprovider.md)ist. Darüber hinaus muss das Profil State-Eigenschaft bereitgestellt werden, bevor er gestartet werden kann. Umfrage Profile-Objekts, um die State-Eigenschaft zu überprüfen.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp | Berechtigungen |
|:-----------|:----------|
| Delegiert (Geschäfts-, Schul- oder Unikonto) | EduAdministration.ReadWrite |
|Delegierte (Persönliches Microsoft-Konto|Nicht unterstützt|
|Anwendung|Nicht unterstützt|

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Wenn nicht erfolgreich ist, es gibt eine `400 Bad Request`. Die Antwort enthält eine Auflistung von [EducationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) -Objekten im Rahmen des Antworttexts, wenn Fehler oder Warnungen gefunden wurden.

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. 

>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2105

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/Collection(microsoft.graph.verificationMessage)",
    "value": [
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have missing data for the field - SIS ID"
        },
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have an invalid format for the field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "125 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "35 row(s) have referenced data not found in source. Field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "10 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "91 row(s) have referenced data not found in source. Field - SIS ID"
        }
    ]
}
```
