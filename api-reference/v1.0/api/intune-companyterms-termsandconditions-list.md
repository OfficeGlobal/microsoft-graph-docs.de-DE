---
title: Auflisten von „termsAndConditions“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditions auf.
author: tfitzmac
ms.openlocfilehash: 8a4d80f0f660a44c1b50d44c7ccebf8f49c891cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330492"
---
# <a name="list-termsandconditionses"></a><span data-ttu-id="a6292-103">Auflisten von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="a6292-103">List termsAndConditionses</span></span>

> <span data-ttu-id="a6292-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a6292-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6292-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) auf.</span><span class="sxs-lookup"><span data-stu-id="a6292-105">List properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6292-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a6292-106">Prerequisites</span></span>
<span data-ttu-id="a6292-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6292-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6292-109">Permission type</span></span>|<span data-ttu-id="a6292-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6292-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6292-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6292-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6292-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6292-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a6292-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6292-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6292-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6292-114">Not supported.</span></span>|
|<span data-ttu-id="a6292-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6292-115">Application</span></span>|<span data-ttu-id="a6292-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6292-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6292-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6292-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="a6292-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6292-118">Request headers</span></span>
|<span data-ttu-id="a6292-119">Header</span><span class="sxs-lookup"><span data-stu-id="a6292-119">Header</span></span>|<span data-ttu-id="a6292-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a6292-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6292-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a6292-121">Authorization</span></span>|<span data-ttu-id="a6292-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a6292-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6292-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a6292-123">Accept</span></span>|<span data-ttu-id="a6292-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a6292-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6292-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6292-125">Request body</span></span>
<span data-ttu-id="a6292-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a6292-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6292-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6292-127">Response</span></span>
<span data-ttu-id="a6292-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a6292-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6292-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6292-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6292-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6292-130">Request</span></span>
<span data-ttu-id="a6292-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6292-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="a6292-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6292-132">Response</span></span>
<span data-ttu-id="a6292-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6292-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7
    }
  ]
}
```



