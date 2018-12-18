---
title: Auflisten von „managedMobileApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedMobileApp auf.
author: tfitzmac
ms.openlocfilehash: c89b6a76be5bee067e02e79353b90e4a7219bc57
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351247"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="c470b-103">Auflisten von „managedMobileApp“</span><span class="sxs-lookup"><span data-stu-id="c470b-103">List managedMobileApps</span></span>

> <span data-ttu-id="c470b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c470b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c470b-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="c470b-105">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c470b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c470b-106">Prerequisites</span></span>
<span data-ttu-id="c470b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c470b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c470b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c470b-109">Permission type</span></span>|<span data-ttu-id="c470b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c470b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c470b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c470b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c470b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c470b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c470b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c470b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c470b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c470b-114">Not supported.</span></span>|
|<span data-ttu-id="c470b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c470b-115">Application</span></span>|<span data-ttu-id="c470b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c470b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c470b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c470b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps
```

## <a name="request-headers"></a><span data-ttu-id="c470b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c470b-118">Request headers</span></span>
|<span data-ttu-id="c470b-119">Header</span><span class="sxs-lookup"><span data-stu-id="c470b-119">Header</span></span>|<span data-ttu-id="c470b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c470b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c470b-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c470b-121">Authorization</span></span>|<span data-ttu-id="c470b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c470b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c470b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c470b-123">Accept</span></span>|<span data-ttu-id="c470b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c470b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c470b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c470b-125">Request body</span></span>
<span data-ttu-id="c470b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c470b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c470b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c470b-127">Response</span></span>
<span data-ttu-id="c470b-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c470b-128">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c470b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c470b-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c470b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c470b-130">Request</span></span>
<span data-ttu-id="c470b-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c470b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="c470b-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c470b-132">Response</span></span>
<span data-ttu-id="c470b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c470b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```



