---
title: Abrufen von „reportRoot“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecfdc13e5e4cdfea5a8c3c9cfb40fe9d6872bd92
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979102"
---
# <a name="get-reportroot"></a><span data-ttu-id="6492b-103">Abrufen von „reportRoot“</span><span class="sxs-lookup"><span data-stu-id="6492b-103">Get reportRoot</span></span>

> <span data-ttu-id="6492b-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="6492b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6492b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6492b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6492b-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6492b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6492b-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="6492b-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6492b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6492b-108">Prerequisites</span></span>
<span data-ttu-id="6492b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6492b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6492b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6492b-111">Permission type</span></span>|<span data-ttu-id="6492b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6492b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6492b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6492b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6492b-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="6492b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6492b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6492b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="6492b-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="6492b-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="6492b-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6492b-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6492b-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6492b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6492b-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6492b-119">Not supported.</span></span>|
|<span data-ttu-id="6492b-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6492b-120">Application</span></span>|<span data-ttu-id="6492b-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6492b-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6492b-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6492b-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6492b-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6492b-123">Optional query parameters</span></span>
<span data-ttu-id="6492b-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6492b-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6492b-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6492b-125">Request headers</span></span>
|<span data-ttu-id="6492b-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6492b-126">Header</span></span>|<span data-ttu-id="6492b-127">Wert</span><span class="sxs-lookup"><span data-stu-id="6492b-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6492b-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6492b-128">Authorization</span></span>|<span data-ttu-id="6492b-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6492b-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6492b-130">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6492b-130">Accept</span></span>|<span data-ttu-id="6492b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="6492b-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6492b-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6492b-132">Request body</span></span>
<span data-ttu-id="6492b-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6492b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6492b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6492b-134">Response</span></span>
<span data-ttu-id="6492b-135">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6492b-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6492b-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6492b-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="6492b-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6492b-137">Request</span></span>
<span data-ttu-id="6492b-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6492b-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="6492b-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6492b-139">Response</span></span>
<span data-ttu-id="6492b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6492b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```



