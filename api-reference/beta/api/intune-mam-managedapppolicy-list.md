---
title: Auflisten von „managedAppPolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedAppPolicy auf.
author: tfitzmac
ms.openlocfilehash: 1883e49cb761861a00be27ed075c841e7a0ee177
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315953"
---
# <a name="list-managedapppolicies"></a><span data-ttu-id="7c9bc-103">Auflisten von „managedAppPolicy“</span><span class="sxs-lookup"><span data-stu-id="7c9bc-103">List managedAppPolicies</span></span>

> <span data-ttu-id="7c9bc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7c9bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c9bc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c9bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c9bc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7c9bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c9bc-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="7c9bc-107">List properties and relationships of the [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c9bc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c9bc-108">Prerequisites</span></span>
<span data-ttu-id="7c9bc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c9bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c9bc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c9bc-111">Permission type</span></span>|<span data-ttu-id="7c9bc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c9bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c9bc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c9bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c9bc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c9bc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7c9bc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c9bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c9bc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c9bc-116">Not supported.</span></span>|
|<span data-ttu-id="7c9bc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c9bc-117">Application</span></span>|<span data-ttu-id="7c9bc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c9bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c9bc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c9bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="7c9bc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c9bc-120">Request headers</span></span>
|<span data-ttu-id="7c9bc-121">Header</span><span class="sxs-lookup"><span data-stu-id="7c9bc-121">Header</span></span>|<span data-ttu-id="7c9bc-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7c9bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c9bc-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="7c9bc-123">Authorization</span></span>|<span data-ttu-id="7c9bc-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c9bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c9bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c9bc-125">Accept</span></span>|<span data-ttu-id="7c9bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c9bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c9bc-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c9bc-127">Request body</span></span>
<span data-ttu-id="7c9bc-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7c9bc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c9bc-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c9bc-129">Response</span></span>
<span data-ttu-id="7c9bc-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c9bc-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c9bc-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c9bc-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c9bc-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c9bc-132">Request</span></span>
<span data-ttu-id="7c9bc-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c9bc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="7c9bc-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c9bc-134">Response</span></span>
<span data-ttu-id="7c9bc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c9bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```





