---
title: Liste androidWorkProfileCustomConfigurations
description: Listeneigenschaften und Beziehungen der AndroidWorkProfileCustomConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 566a04b1d732dab6b765876f8b1823a1c640ee6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850897"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="2fd4d-103">Liste androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="2fd4d-103">List androidWorkProfileCustomConfigurations</span></span>

> <span data-ttu-id="2fd4d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fd4d-105">Listeneigenschaften und Beziehungen der [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-105">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2fd4d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2fd4d-106">Prerequisites</span></span>
<span data-ttu-id="2fd4d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fd4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fd4d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2fd4d-109">Permission type</span></span>|<span data-ttu-id="2fd4d-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2fd4d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fd4d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2fd4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2fd4d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fd4d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2fd4d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2fd4d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fd4d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2fd4d-114">Not supported.</span></span>|
|<span data-ttu-id="2fd4d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2fd4d-115">Application</span></span>|<span data-ttu-id="2fd4d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2fd4d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fd4d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2fd4d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2fd4d-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2fd4d-118">Request headers</span></span>
|<span data-ttu-id="2fd4d-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2fd4d-119">Header</span></span>|<span data-ttu-id="2fd4d-120">Wert</span><span class="sxs-lookup"><span data-stu-id="2fd4d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fd4d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fd4d-121">Authorization</span></span>|<span data-ttu-id="2fd4d-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2fd4d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fd4d-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2fd4d-123">Accept</span></span>|<span data-ttu-id="2fd4d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2fd4d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fd4d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2fd4d-125">Request body</span></span>
<span data-ttu-id="2fd4d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fd4d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2fd4d-127">Response</span></span>
<span data-ttu-id="2fd4d-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2fd4d-128">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fd4d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2fd4d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2fd4d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2fd4d-130">Request</span></span>
<span data-ttu-id="2fd4d-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2fd4d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2fd4d-132">Response</span></span>
<span data-ttu-id="2fd4d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2fd4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



