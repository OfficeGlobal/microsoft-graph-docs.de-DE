---
title: appleDeviceFeaturesConfigurationBase abrufen
description: Lesen der Eigenschaften und Beziehungen des appleDeviceFeaturesConfigurationBase-Objekts.
author: tfitzmac
ms.openlocfilehash: 096291a17ded6afc90816d862eb1ae1bcc8408e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312418"
---
# <a name="get-appledevicefeaturesconfigurationbase"></a><span data-ttu-id="b1bca-103">appleDeviceFeaturesConfigurationBase abrufen</span><span class="sxs-lookup"><span data-stu-id="b1bca-103">Get appleDeviceFeaturesConfigurationBase</span></span>

> <span data-ttu-id="b1bca-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b1bca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1bca-105">Lesen der Eigenschaften und Beziehungen des [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="b1bca-105">Read properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1bca-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b1bca-106">Prerequisites</span></span>
<span data-ttu-id="b1bca-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1bca-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1bca-109">Permission type</span></span>|<span data-ttu-id="b1bca-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1bca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1bca-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1bca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1bca-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1bca-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b1bca-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1bca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1bca-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1bca-114">Not supported.</span></span>|
|<span data-ttu-id="b1bca-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1bca-115">Application</span></span>|<span data-ttu-id="b1bca-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1bca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1bca-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1bca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1bca-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b1bca-118">Optional query parameters</span></span>
<span data-ttu-id="b1bca-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b1bca-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1bca-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1bca-120">Request headers</span></span>
|<span data-ttu-id="b1bca-121">Header</span><span class="sxs-lookup"><span data-stu-id="b1bca-121">Header</span></span>|<span data-ttu-id="b1bca-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b1bca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1bca-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b1bca-123">Authorization</span></span>|<span data-ttu-id="b1bca-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b1bca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1bca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b1bca-125">Accept</span></span>|<span data-ttu-id="b1bca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1bca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1bca-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1bca-127">Request body</span></span>
<span data-ttu-id="b1bca-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b1bca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1bca-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1bca-129">Response</span></span>
<span data-ttu-id="b1bca-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1bca-130">If successful, this method returns a `200 OK` response code and [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1bca-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1bca-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1bca-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1bca-132">Request</span></span>
<span data-ttu-id="b1bca-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1bca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b1bca-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1bca-134">Response</span></span>
<span data-ttu-id="b1bca-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1bca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "value": {
    "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
    "id": "ca0bb5ff-b5ff-ca0b-ffb5-0bcaffb50bca",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



