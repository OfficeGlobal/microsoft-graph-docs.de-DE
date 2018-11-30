---
title: Auflisten von „targetedManagedAppConfiguration“
description: Auflisten von Eigenschaften und Beziehungen der targetedManagedAppConfiguration-Objekte.
ms.openlocfilehash: b0c4d2c16e9971c64c9dc674a233735de8be4b90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016164"
---
# <a name="list-targetedmanagedappconfigurations"></a><span data-ttu-id="66930-103">Auflisten von „targetedManagedAppConfiguration“</span><span class="sxs-lookup"><span data-stu-id="66930-103">List targetedManagedAppConfigurations</span></span>

> <span data-ttu-id="66930-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="66930-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66930-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="66930-105">List properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66930-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="66930-106">Prerequisites</span></span>
<span data-ttu-id="66930-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66930-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66930-109">Permission type</span></span>|<span data-ttu-id="66930-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66930-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66930-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66930-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66930-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="66930-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="66930-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66930-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66930-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66930-114">Not supported.</span></span>|
|<span data-ttu-id="66930-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66930-115">Application</span></span>|<span data-ttu-id="66930-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66930-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66930-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66930-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="66930-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66930-118">Request headers</span></span>
|<span data-ttu-id="66930-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="66930-119">Header</span></span>|<span data-ttu-id="66930-120">Wert</span><span class="sxs-lookup"><span data-stu-id="66930-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66930-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66930-121">Authorization</span></span>|<span data-ttu-id="66930-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="66930-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66930-123">Accept</span><span class="sxs-lookup"><span data-stu-id="66930-123">Accept</span></span>|<span data-ttu-id="66930-124">application/json</span><span class="sxs-lookup"><span data-stu-id="66930-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66930-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66930-125">Request body</span></span>
<span data-ttu-id="66930-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="66930-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66930-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="66930-127">Response</span></span>
<span data-ttu-id="66930-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="66930-128">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66930-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66930-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="66930-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66930-130">Request</span></span>
<span data-ttu-id="66930-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66930-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
```

### <a name="response"></a><span data-ttu-id="66930-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="66930-132">Response</span></span>
<span data-ttu-id="66930-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66930-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



