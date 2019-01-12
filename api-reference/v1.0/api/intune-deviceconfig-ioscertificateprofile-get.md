---
title: iosCertificateProfile abrufen
description: Lesen von Eigenschaften und Beziehungen des iosCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b4a3d7f4e6fc2a38964d740fe94a4ad4a71c6374
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983526"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="748bd-103">iosCertificateProfile abrufen</span><span class="sxs-lookup"><span data-stu-id="748bd-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="748bd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="748bd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="748bd-105">Lesen von Eigenschaften und Beziehungen des [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="748bd-105">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="748bd-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="748bd-106">Prerequisites</span></span>
<span data-ttu-id="748bd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="748bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="748bd-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="748bd-109">Permission type</span></span>|<span data-ttu-id="748bd-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="748bd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="748bd-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="748bd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="748bd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="748bd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="748bd-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="748bd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="748bd-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="748bd-114">Not supported.</span></span>|
|<span data-ttu-id="748bd-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="748bd-115">Application</span></span>|<span data-ttu-id="748bd-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="748bd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="748bd-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="748bd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="748bd-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="748bd-118">Optional query parameters</span></span>
<span data-ttu-id="748bd-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="748bd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="748bd-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="748bd-120">Request headers</span></span>
|<span data-ttu-id="748bd-121">Header</span><span class="sxs-lookup"><span data-stu-id="748bd-121">Header</span></span>|<span data-ttu-id="748bd-122">Wert</span><span class="sxs-lookup"><span data-stu-id="748bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="748bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="748bd-123">Authorization</span></span>|<span data-ttu-id="748bd-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="748bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="748bd-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="748bd-125">Accept</span></span>|<span data-ttu-id="748bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="748bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="748bd-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="748bd-127">Request body</span></span>
<span data-ttu-id="748bd-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="748bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="748bd-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="748bd-129">Response</span></span>
<span data-ttu-id="748bd-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="748bd-130">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="748bd-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="748bd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="748bd-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="748bd-132">Request</span></span>
<span data-ttu-id="748bd-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="748bd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="748bd-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="748bd-134">Response</span></span>
<span data-ttu-id="748bd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="748bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 364

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



