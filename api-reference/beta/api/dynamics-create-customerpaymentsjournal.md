---
title: CustomerPaymentJournals erstellen
description: Erstellt ein Kunden Zahlungsjournal-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a633ef91fe15b4999285d7290ca6eed8c10846a3
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365465"
---
# <a name="create-customerpaymentjournals"></a>CustomerPaymentJournals erstellen
Erstellt ein Kunden-Zahlungsjournal Objekt in Dynamics 365 Business Central.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp |Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)|
|:---------------|:------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|Financials.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto|Nicht unterstützt|
|Anwendung|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-Anforderung

```
POST /financials/companies('{id}')/customerPaymentJournals('{id}')
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile        |Wert                    |
|--------------|-------------------------|
|Authorization |Bearer {token}. Erforderlich.|
|Content-Type  |application/json         |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung des **customerPaymentJournals** -Objekts an.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und ein **customerPaymentJournals** -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

**Anforderung**

Hier ist ein Beispiel für eine Anforderung.

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

**Antwort**

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


