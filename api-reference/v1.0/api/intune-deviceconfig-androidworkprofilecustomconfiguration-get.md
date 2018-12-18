---
title: Abrufen von androidWorkProfileCustomConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des AndroidWorkProfileCustomConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: 4e12962e59bc45635b202aeda08e7e8c299bc51c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328567"
---
# <a name="get-androidworkprofilecustomconfiguration"></a><span data-ttu-id="22c71-103">Abrufen von androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="22c71-103">Get androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="22c71-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="22c71-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22c71-105">Lesen Sie Eigenschaften und Beziehungen des [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="22c71-105">Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22c71-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="22c71-106">Prerequisites</span></span>
<span data-ttu-id="22c71-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22c71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22c71-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22c71-109">Permission type</span></span>|<span data-ttu-id="22c71-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22c71-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22c71-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22c71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="22c71-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22c71-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22c71-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22c71-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22c71-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22c71-114">Not supported.</span></span>|
|<span data-ttu-id="22c71-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22c71-115">Application</span></span>|<span data-ttu-id="22c71-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22c71-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22c71-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22c71-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22c71-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="22c71-118">Optional query parameters</span></span>
<span data-ttu-id="22c71-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="22c71-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="22c71-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22c71-120">Request headers</span></span>
|<span data-ttu-id="22c71-121">Header</span><span class="sxs-lookup"><span data-stu-id="22c71-121">Header</span></span>|<span data-ttu-id="22c71-122">Wert</span><span class="sxs-lookup"><span data-stu-id="22c71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22c71-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="22c71-123">Authorization</span></span>|<span data-ttu-id="22c71-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="22c71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22c71-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22c71-125">Accept</span></span>|<span data-ttu-id="22c71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22c71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22c71-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22c71-127">Request body</span></span>
<span data-ttu-id="22c71-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="22c71-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22c71-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="22c71-129">Response</span></span>
<span data-ttu-id="22c71-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="22c71-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22c71-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22c71-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="22c71-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22c71-132">Request</span></span>
<span data-ttu-id="22c71-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22c71-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="22c71-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="22c71-134">Response</span></span>
<span data-ttu-id="22c71-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22c71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 636

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
    "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "omaSettings": [
      {
        "@odata.type": "microsoft.graph.omaSettingInteger",
        "displayName": "Display Name value",
        "description": "Description value",
        "omaUri": "Oma Uri value",
        "value": 5
      }
    ]
  }
}
```



