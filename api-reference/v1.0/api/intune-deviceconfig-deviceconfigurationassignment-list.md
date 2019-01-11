---
title: Auflisten von „deviceConfigurationAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceConfigurationAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 88ae5ad2e007096eb8853d522f780d272d71a3a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867403"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="1ac53-103">Auflisten von „deviceConfigurationAssignment“</span><span class="sxs-lookup"><span data-stu-id="1ac53-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="1ac53-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1ac53-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ac53-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="1ac53-105">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ac53-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1ac53-106">Prerequisites</span></span>
<span data-ttu-id="1ac53-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ac53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ac53-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ac53-109">Permission type</span></span>|<span data-ttu-id="1ac53-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ac53-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ac53-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ac53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ac53-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ac53-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ac53-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ac53-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ac53-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ac53-114">Not supported.</span></span>|
|<span data-ttu-id="1ac53-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ac53-115">Application</span></span>|<span data-ttu-id="1ac53-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ac53-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ac53-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ac53-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1ac53-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ac53-118">Request headers</span></span>
|<span data-ttu-id="1ac53-119">Header</span><span class="sxs-lookup"><span data-stu-id="1ac53-119">Header</span></span>|<span data-ttu-id="1ac53-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1ac53-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ac53-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ac53-121">Authorization</span></span>|<span data-ttu-id="1ac53-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1ac53-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ac53-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1ac53-123">Accept</span></span>|<span data-ttu-id="1ac53-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ac53-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ac53-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ac53-125">Request body</span></span>
<span data-ttu-id="1ac53-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1ac53-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ac53-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ac53-127">Response</span></span>
<span data-ttu-id="1ac53-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1ac53-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ac53-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ac53-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ac53-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ac53-130">Request</span></span>
<span data-ttu-id="1ac53-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ac53-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="1ac53-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ac53-132">Response</span></span>
<span data-ttu-id="1ac53-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ac53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



