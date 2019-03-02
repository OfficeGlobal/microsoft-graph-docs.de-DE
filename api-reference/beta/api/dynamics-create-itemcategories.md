---
title: ItemCategories erstellen
description: Erstellt ein Element Category-Objekt in Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 6d3e2918854e169c13971d0c71fc66091874d3ab
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365388"
---
# <a name="create-itemcategories"></a>ItemCategories erstellen
Erstellen Sie ein Element Category-Objekt Dynamics 365 Business Central.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp |Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)|
|:---------------|:------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)|Financials.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto|Nicht unterstützt|
|Anwendung|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-Anforderung
```
POST /financials/companies('{id}')/itemCategories
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
|Kopfzeile       |Wert                    |
|-------------|-------------------------|
|Authorization|Bearer {token}. Erforderlich.|
|Content-Type |application/json         |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung eines **itemCategories** -Objekts an.

## <a name="response"></a>Antwort
Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und ein **itemCategories** -Objekt im Antworttext zurück.

## <a name="example"></a>Beispiel

**Anforderung**

Hier ist ein Beispiel für eine Anforderung.

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

**Antwort**

Nachfolgend sehen Sie ein Beispiel der Antwort. 

> **Hinweis**: das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}

```




