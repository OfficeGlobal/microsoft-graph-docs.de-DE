---
title: managedMobileApp abrufen
description: Lesen von Eigenschaften und Beziehungen des managedMobileApp-Objekts.
ms.openlocfilehash: ea5fe4a4f69c3b2237770e4036d09476f6fdf52a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016753"
---
# <a name="get-managedmobileapp"></a><span data-ttu-id="e5943-103">managedMobileApp abrufen</span><span class="sxs-lookup"><span data-stu-id="e5943-103">Get managedMobileApp</span></span>

> <span data-ttu-id="e5943-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e5943-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5943-105">Lesen von Eigenschaften und Beziehungen des [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e5943-105">Read properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5943-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e5943-106">Prerequisites</span></span>
<span data-ttu-id="e5943-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5943-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5943-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e5943-109">Permission type</span></span>|<span data-ttu-id="e5943-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e5943-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5943-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e5943-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5943-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5943-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e5943-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e5943-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5943-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5943-114">Not supported.</span></span>|
|<span data-ttu-id="e5943-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e5943-115">Application</span></span>|<span data-ttu-id="e5943-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e5943-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5943-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5943-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5943-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e5943-118">Optional query parameters</span></span>
<span data-ttu-id="e5943-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e5943-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e5943-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e5943-120">Request headers</span></span>
|<span data-ttu-id="e5943-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e5943-121">Header</span></span>|<span data-ttu-id="e5943-122">Wert</span><span class="sxs-lookup"><span data-stu-id="e5943-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5943-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5943-123">Authorization</span></span>|<span data-ttu-id="e5943-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e5943-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5943-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5943-125">Accept</span></span>|<span data-ttu-id="e5943-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5943-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5943-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e5943-127">Request body</span></span>
<span data-ttu-id="e5943-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e5943-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5943-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5943-129">Response</span></span>
<span data-ttu-id="e5943-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [managedMobileApp](../resources/intune-mam-managedmobileapp.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5943-130">If successful, this method returns a `200 OK` response code and [managedMobileApp](../resources/intune-mam-managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5943-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e5943-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5943-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e5943-132">Request</span></span>
<span data-ttu-id="e5943-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e5943-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
```

### <a name="response"></a><span data-ttu-id="e5943-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e5943-134">Response</span></span>
<span data-ttu-id="e5943-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e5943-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.managedMobileApp",
    "mobileAppIdentifier": {
      "@odata.type": "microsoft.graph.mobileAppIdentifier"
    },
    "id": "0a129715-9715-0a12-1597-120a1597120a",
    "version": "Version value"
  }
}
```



