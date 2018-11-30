---
title: iosCertificateProfile abrufen
description: Lesen von Eigenschaften und Beziehungen des iosCertificateProfile-Objekts.
ms.openlocfilehash: fb0cbb214f79c5621c093da9dff4b82ad9021f46
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018067"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="000c3-103">iosCertificateProfile abrufen</span><span class="sxs-lookup"><span data-stu-id="000c3-103">Get iosCertificateProfile</span></span>

> <span data-ttu-id="000c3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="000c3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="000c3-105">Lesen von Eigenschaften und Beziehungen des [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="000c3-105">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="000c3-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="000c3-106">Prerequisites</span></span>
<span data-ttu-id="000c3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="000c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="000c3-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="000c3-109">Permission type</span></span>|<span data-ttu-id="000c3-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="000c3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="000c3-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="000c3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="000c3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="000c3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="000c3-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="000c3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="000c3-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="000c3-114">Not supported.</span></span>|
|<span data-ttu-id="000c3-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="000c3-115">Application</span></span>|<span data-ttu-id="000c3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="000c3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="000c3-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="000c3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="000c3-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="000c3-118">Optional query parameters</span></span>
<span data-ttu-id="000c3-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="000c3-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="000c3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="000c3-120">Request headers</span></span>
|<span data-ttu-id="000c3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="000c3-121">Header</span></span>|<span data-ttu-id="000c3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="000c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="000c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="000c3-123">Authorization</span></span>|<span data-ttu-id="000c3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="000c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="000c3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="000c3-125">Accept</span></span>|<span data-ttu-id="000c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="000c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="000c3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="000c3-127">Request body</span></span>
<span data-ttu-id="000c3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="000c3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="000c3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="000c3-129">Response</span></span>
<span data-ttu-id="000c3-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="000c3-130">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="000c3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="000c3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="000c3-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="000c3-132">Request</span></span>
<span data-ttu-id="000c3-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="000c3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="000c3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="000c3-134">Response</span></span>
<span data-ttu-id="000c3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="000c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


