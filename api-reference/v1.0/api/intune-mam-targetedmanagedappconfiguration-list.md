---
title: Auflisten von „targetedManagedAppConfiguration“
description: Auflisten von Eigenschaften und Beziehungen der targetedManagedAppConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac6351591e554f0535eb34817c170453b1d41b80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957032"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="6243e-103">Auflisten von „targetedManagedAppConfiguration“</span><span class="sxs-lookup"><span data-stu-id="6243e-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="6243e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6243e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6243e-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="6243e-105">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6243e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6243e-106">Prerequisites</span></span>
<span data-ttu-id="6243e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6243e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6243e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6243e-109">Permission type</span></span>|<span data-ttu-id="6243e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6243e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6243e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6243e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6243e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6243e-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6243e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6243e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6243e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6243e-114">Not supported.</span></span>|
|<span data-ttu-id="6243e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6243e-115">Application</span></span>|<span data-ttu-id="6243e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6243e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6243e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6243e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6243e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6243e-118">Request headers</span></span>
|<span data-ttu-id="6243e-119">Header</span><span class="sxs-lookup"><span data-stu-id="6243e-119">Header</span></span>|<span data-ttu-id="6243e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6243e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6243e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6243e-121">Authorization</span></span>|<span data-ttu-id="6243e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6243e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6243e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6243e-123">Accept</span></span>|<span data-ttu-id="6243e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6243e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6243e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6243e-125">Request body</span></span>
<span data-ttu-id="6243e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6243e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6243e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="6243e-127">Response</span></span>
<span data-ttu-id="6243e-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6243e-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6243e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6243e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6243e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6243e-130">Request</span></span>
<span data-ttu-id="6243e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6243e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="6243e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="6243e-132">Response</span></span>
<span data-ttu-id="6243e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6243e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 657

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "2444e029-e029-2444-29e0-442429e04424",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "deployedAppCount": 0,
      "isAssigned": true
    }
  ]
}
```



