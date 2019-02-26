---
title: Auflisten von „termsAndConditionsAcceptanceStatus“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditionsAcceptanceStatus auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2fdccc1ab2376aa922ce866adce8c8081c9c28e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263259"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="c1234-103">Auflisten von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="c1234-103">List termsAndConditionsAcceptanceStatuses</span></span>

> <span data-ttu-id="c1234-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c1234-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1234-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) auf.</span><span class="sxs-lookup"><span data-stu-id="c1234-105">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1234-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c1234-106">Prerequisites</span></span>
<span data-ttu-id="c1234-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c1234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1234-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c1234-109">Permission type</span></span>|<span data-ttu-id="c1234-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c1234-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1234-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c1234-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c1234-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1234-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c1234-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c1234-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1234-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1234-114">Not supported.</span></span>|
|<span data-ttu-id="c1234-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c1234-115">Application</span></span>|<span data-ttu-id="c1234-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c1234-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1234-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1234-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c1234-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c1234-118">Request headers</span></span>
|<span data-ttu-id="c1234-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c1234-119">Header</span></span>|<span data-ttu-id="c1234-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c1234-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1234-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1234-121">Authorization</span></span>|<span data-ttu-id="c1234-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c1234-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1234-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c1234-123">Accept</span></span>|<span data-ttu-id="c1234-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c1234-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1234-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c1234-125">Request body</span></span>
<span data-ttu-id="c1234-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c1234-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1234-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1234-127">Response</span></span>
<span data-ttu-id="c1234-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c1234-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1234-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c1234-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1234-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c1234-130">Request</span></span>
<span data-ttu-id="c1234-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c1234-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="c1234-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c1234-132">Response</span></span>
<span data-ttu-id="c1234-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c1234-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
      "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
      "userDisplayName": "User Display Name value",
      "acceptedVersion": 15,
      "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
    }
  ]
}
```



