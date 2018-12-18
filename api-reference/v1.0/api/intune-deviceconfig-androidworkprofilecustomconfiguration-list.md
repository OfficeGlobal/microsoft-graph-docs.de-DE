---
title: Liste androidWorkProfileCustomConfigurations
description: Listeneigenschaften und Beziehungen der AndroidWorkProfileCustomConfiguration-Objekte.
author: tfitzmac
ms.openlocfilehash: b81e25f4168c41d9859d9e142ddf195ade7fd598
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358884"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="b3226-103">Liste androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="b3226-103">List androidWorkProfileCustomConfigurations</span></span>

> <span data-ttu-id="b3226-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b3226-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3226-105">Listeneigenschaften und Beziehungen der [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b3226-105">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3226-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b3226-106">Prerequisites</span></span>
<span data-ttu-id="b3226-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3226-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3226-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b3226-109">Permission type</span></span>|<span data-ttu-id="b3226-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b3226-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3226-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b3226-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b3226-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3226-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b3226-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b3226-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3226-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3226-114">Not supported.</span></span>|
|<span data-ttu-id="b3226-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b3226-115">Application</span></span>|<span data-ttu-id="b3226-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b3226-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3226-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3226-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b3226-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b3226-118">Request headers</span></span>
|<span data-ttu-id="b3226-119">Header</span><span class="sxs-lookup"><span data-stu-id="b3226-119">Header</span></span>|<span data-ttu-id="b3226-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b3226-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3226-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b3226-121">Authorization</span></span>|<span data-ttu-id="b3226-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b3226-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3226-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b3226-123">Accept</span></span>|<span data-ttu-id="b3226-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3226-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3226-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b3226-125">Request body</span></span>
<span data-ttu-id="b3226-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b3226-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3226-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3226-127">Response</span></span>
<span data-ttu-id="b3226-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b3226-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3226-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b3226-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3226-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b3226-130">Request</span></span>
<span data-ttu-id="b3226-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b3226-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b3226-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="b3226-132">Response</span></span>
<span data-ttu-id="b3226-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b3226-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 682

{
  "value": [
    {
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
  ]
}
```



