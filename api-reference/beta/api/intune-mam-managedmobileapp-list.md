---
title: Auflisten von „managedMobileApp“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedMobileApp auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 90ddc72971c108fb3cb4a792204d5bae794f5b11
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970632"
---
# <a name="list-managedmobileapps"></a><span data-ttu-id="5247b-103">Auflisten von „managedMobileApp“</span><span class="sxs-lookup"><span data-stu-id="5247b-103">List managedMobileApps</span></span>

> <span data-ttu-id="5247b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5247b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5247b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5247b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5247b-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) auf.</span><span class="sxs-lookup"><span data-stu-id="5247b-106">List properties and relationships of the [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5247b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5247b-107">Prerequisites</span></span>
<span data-ttu-id="5247b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5247b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5247b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5247b-110">Permission type</span></span>|<span data-ttu-id="5247b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5247b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5247b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5247b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5247b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5247b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5247b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5247b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5247b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5247b-115">Not supported.</span></span>|
|<span data-ttu-id="5247b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5247b-116">Application</span></span>|<span data-ttu-id="5247b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5247b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5247b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5247b-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5247b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5247b-119">Request headers</span></span>
|<span data-ttu-id="5247b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5247b-120">Header</span></span>|<span data-ttu-id="5247b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5247b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5247b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5247b-122">Authorization</span></span>|<span data-ttu-id="5247b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5247b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5247b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5247b-124">Accept</span></span>|<span data-ttu-id="5247b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5247b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5247b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5247b-126">Request body</span></span>
<span data-ttu-id="5247b-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5247b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5247b-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="5247b-128">Response</span></span>
<span data-ttu-id="5247b-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedMobileApp](../resources/intune-mam-managedmobileapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5247b-129">If successful, this method returns a `200 OK` response code and a collection of [managedMobileApp](../resources/intune-mam-managedmobileapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5247b-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5247b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5247b-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5247b-131">Request</span></span>
<span data-ttu-id="5247b-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5247b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps
```

### <a name="response"></a><span data-ttu-id="5247b-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5247b-133">Response</span></span>
<span data-ttu-id="5247b-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5247b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




