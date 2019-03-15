---
title: AndroidManagedStoreAppConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des androidManagedStoreAppConfiguration-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b884077e602d02b6302c8ba36a7339e82e761d53
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571599"
---
# <a name="get-androidmanagedstoreappconfiguration"></a><span data-ttu-id="901e5-103">AndroidManagedStoreAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="901e5-103">Get androidManagedStoreAppConfiguration</span></span>

> <span data-ttu-id="901e5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="901e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="901e5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="901e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="901e5-106">Lesen von Eigenschaften und Beziehungen des [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="901e5-106">Read properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="901e5-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="901e5-107">Prerequisites</span></span>
<span data-ttu-id="901e5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="901e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="901e5-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="901e5-110">Permission type</span></span>|<span data-ttu-id="901e5-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="901e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="901e5-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="901e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="901e5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="901e5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="901e5-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="901e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="901e5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="901e5-115">Not supported.</span></span>|
|<span data-ttu-id="901e5-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="901e5-116">Application</span></span>|<span data-ttu-id="901e5-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="901e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="901e5-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="901e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="901e5-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="901e5-119">Optional query parameters</span></span>
<span data-ttu-id="901e5-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="901e5-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="901e5-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="901e5-121">Request headers</span></span>
|<span data-ttu-id="901e5-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="901e5-122">Header</span></span>|<span data-ttu-id="901e5-123">Wert</span><span class="sxs-lookup"><span data-stu-id="901e5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="901e5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="901e5-124">Authorization</span></span>|<span data-ttu-id="901e5-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="901e5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="901e5-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="901e5-126">Accept</span></span>|<span data-ttu-id="901e5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="901e5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="901e5-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="901e5-128">Request body</span></span>
<span data-ttu-id="901e5-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="901e5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="901e5-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="901e5-130">Response</span></span>
<span data-ttu-id="901e5-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="901e5-131">If successful, this method returns a `200 OK` response code and [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="901e5-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="901e5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="901e5-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="901e5-133">Request</span></span>
<span data-ttu-id="901e5-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="901e5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="901e5-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="901e5-135">Response</span></span>
<span data-ttu-id="901e5-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="901e5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 829

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
    "id": "919a9335-9335-919a-3593-9a9135939a91",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "packageId": "Package Id value",
    "payloadJson": "Payload Json value",
    "permissionActions": [
      {
        "@odata.type": "microsoft.graph.androidPermissionAction",
        "permission": "Permission value",
        "action": "autoGrant"
      }
    ],
    "appSupportsOemConfig": true
  }
}
```




