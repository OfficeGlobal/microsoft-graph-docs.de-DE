---
title: TaxAreas erstellen
description: Erstellt ein Steuerbereich-Objekt in Dynamics für Financials.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 6addfb3617b05bcb8b6a12d6df31e115d5ea01a9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365766"
---
# <a name="create-taxareas"></a><span data-ttu-id="0b6e0-103">TaxAreas erstellen</span><span class="sxs-lookup"><span data-stu-id="0b6e0-103">Create taxAreas</span></span>
<span data-ttu-id="0b6e0-104">Erstellt ein Steuerbereich-Objekt in Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="0b6e0-104">Creates a tax area object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b6e0-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0b6e0-105">Permissions</span></span>
<span data-ttu-id="0b6e0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b6e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b6e0-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b6e0-108">Permission type</span></span> |<span data-ttu-id="0b6e0-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b6e0-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="0b6e0-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b6e0-110">Delegated (work or school account)</span></span>|<span data-ttu-id="0b6e0-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b6e0-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="0b6e0-112">Delegiert (persönliches Microsoft-Konto</span><span class="sxs-lookup"><span data-stu-id="0b6e0-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="0b6e0-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b6e0-113">Not supported.</span></span>|
|<span data-ttu-id="0b6e0-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b6e0-114">Application</span></span>|<span data-ttu-id="0b6e0-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b6e0-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b6e0-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b6e0-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/taxAreas('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b6e0-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0b6e0-117">Optional query parameters</span></span>
<span data-ttu-id="0b6e0-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0b6e0-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b6e0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b6e0-119">Request headers</span></span>
|<span data-ttu-id="0b6e0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0b6e0-120">Header</span></span>|<span data-ttu-id="0b6e0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0b6e0-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="0b6e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b6e0-122">Authorization</span></span>  |<span data-ttu-id="0b6e0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0b6e0-p102">Bearer {token}. Required.</span></span>    |
|<span data-ttu-id="0b6e0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0b6e0-125">Content-Type</span></span>  |<span data-ttu-id="0b6e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b6e0-126">application/json</span></span>    |

## <a name="request-body"></a><span data-ttu-id="0b6e0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b6e0-127">Request body</span></span>
<span data-ttu-id="0b6e0-128">Geben Sie im Anforderungstext eine JSON-Darstellung eines **taxAreas** -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0b6e0-128">In the request body, supply a JSON representation of a **taxAreas** object.</span></span>

## <a name="response"></a><span data-ttu-id="0b6e0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b6e0-129">Response</span></span>
<span data-ttu-id="0b6e0-130">Bei erfolgreicher Ausführung gibt diese Methode ```201 Created``` den Antwortcode und ein **taxAreas** -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0b6e0-130">If successful, this method returns ```201 Created``` response code and a **taxAreas** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b6e0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b6e0-131">Example</span></span>

<span data-ttu-id="0b6e0-132">**Anforderung**</span><span class="sxs-lookup"><span data-stu-id="0b6e0-132">**Request**</span></span>

<span data-ttu-id="0b6e0-133">Hier ist ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b6e0-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/taxAreas
Content-type: application/json

```json
{
  "code": "44442001T"
}
```

<span data-ttu-id="0b6e0-134">**Antwort**</span><span class="sxs-lookup"><span data-stu-id="0b6e0-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "44442001T",
  "displayName": "tax area",
  "taxType": "Sales Tax",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```
