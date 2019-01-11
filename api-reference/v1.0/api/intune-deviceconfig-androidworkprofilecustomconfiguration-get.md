---
title: Abrufen von androidWorkProfileCustomConfiguration
description: Lesen Sie Eigenschaften und Beziehungen des AndroidWorkProfileCustomConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e966d803a801ff07c91accfea99aac40a99e28c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881109"
---
# <a name="get-androidworkprofilecustomconfiguration"></a><span data-ttu-id="7d774-103">Abrufen von androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d774-103">Get androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="7d774-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7d774-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d774-105">Lesen Sie Eigenschaften und Beziehungen des [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="7d774-105">Read properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d774-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7d774-106">Prerequisites</span></span>
<span data-ttu-id="7d774-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d774-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d774-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7d774-109">Permission type</span></span>|<span data-ttu-id="7d774-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7d774-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d774-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7d774-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d774-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7d774-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7d774-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7d774-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d774-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d774-114">Not supported.</span></span>|
|<span data-ttu-id="7d774-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7d774-115">Application</span></span>|<span data-ttu-id="7d774-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d774-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d774-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d774-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d774-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7d774-118">Optional query parameters</span></span>
<span data-ttu-id="7d774-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7d774-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7d774-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7d774-120">Request headers</span></span>
|<span data-ttu-id="7d774-121">Header</span><span class="sxs-lookup"><span data-stu-id="7d774-121">Header</span></span>|<span data-ttu-id="7d774-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7d774-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d774-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d774-123">Authorization</span></span>|<span data-ttu-id="7d774-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7d774-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d774-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7d774-125">Accept</span></span>|<span data-ttu-id="7d774-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d774-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d774-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7d774-127">Request body</span></span>
<span data-ttu-id="7d774-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7d774-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d774-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d774-129">Response</span></span>
<span data-ttu-id="7d774-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="7d774-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d774-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7d774-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d774-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d774-132">Request</span></span>
<span data-ttu-id="7d774-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7d774-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7d774-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d774-134">Response</span></span>
<span data-ttu-id="7d774-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7d774-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



