---
title: Liste locationManagementConditions
description: Listeneigenschaften und Beziehungen der LocationManagementCondition-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0a5f02a8e3329b2b903d378eb609d5cc0e94e784
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969870"
---
# <a name="list-locationmanagementconditions"></a><span data-ttu-id="c6108-103">Liste locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="c6108-103">List locationManagementConditions</span></span>

> <span data-ttu-id="c6108-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c6108-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6108-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c6108-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6108-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c6108-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6108-107">Listeneigenschaften und Beziehungen der [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="c6108-107">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6108-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c6108-108">Prerequisites</span></span>
<span data-ttu-id="c6108-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6108-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6108-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6108-111">Permission type</span></span>|<span data-ttu-id="c6108-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6108-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6108-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6108-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6108-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6108-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c6108-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6108-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6108-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6108-116">Not supported.</span></span>|
|<span data-ttu-id="c6108-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6108-117">Application</span></span>|<span data-ttu-id="c6108-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c6108-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6108-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6108-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="c6108-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6108-120">Request headers</span></span>
|<span data-ttu-id="c6108-121">Header</span><span class="sxs-lookup"><span data-stu-id="c6108-121">Header</span></span>|<span data-ttu-id="c6108-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c6108-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6108-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6108-123">Authorization</span></span>|<span data-ttu-id="c6108-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c6108-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6108-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c6108-125">Accept</span></span>|<span data-ttu-id="c6108-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6108-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6108-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c6108-127">Request body</span></span>
<span data-ttu-id="c6108-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c6108-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6108-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6108-129">Response</span></span>
<span data-ttu-id="c6108-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [LocationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="c6108-130">If successful, this method returns a `200 OK` response code and a collection of [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6108-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6108-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6108-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6108-132">Request</span></span>
<span data-ttu-id="c6108-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c6108-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="c6108-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6108-134">Response</span></span>
<span data-ttu-id="c6108-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6108-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.locationManagementCondition",
      "id": "23b1ca32-ca32-23b1-32ca-b12332cab123",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```





