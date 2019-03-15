---
title: AndroidManagedStoreAppConfigurations aufListen
description: AufListen von Eigenschaften und Beziehungen der androidManagedStoreAppConfiguration-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7df116f50c0b3f0c35e85af5e25b8b57eed223bd
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570948"
---
# <a name="list-androidmanagedstoreappconfigurations"></a><span data-ttu-id="b84c4-103">AndroidManagedStoreAppConfigurations aufListen</span><span class="sxs-lookup"><span data-stu-id="b84c4-103">List androidManagedStoreAppConfigurations</span></span>

> <span data-ttu-id="b84c4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b84c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b84c4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b84c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b84c4-106">AufListen von Eigenschaften und Beziehungen der [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b84c4-106">List properties and relationships of the [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b84c4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b84c4-107">Prerequisites</span></span>
<span data-ttu-id="b84c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b84c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b84c4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b84c4-110">Permission type</span></span>|<span data-ttu-id="b84c4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b84c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b84c4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b84c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b84c4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b84c4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b84c4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b84c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b84c4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b84c4-115">Not supported.</span></span>|
|<span data-ttu-id="b84c4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b84c4-116">Application</span></span>|<span data-ttu-id="b84c4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b84c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b84c4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b84c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b84c4-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b84c4-119">Request headers</span></span>
|<span data-ttu-id="b84c4-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b84c4-120">Header</span></span>|<span data-ttu-id="b84c4-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b84c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b84c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b84c4-122">Authorization</span></span>|<span data-ttu-id="b84c4-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b84c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b84c4-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b84c4-124">Accept</span></span>|<span data-ttu-id="b84c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b84c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b84c4-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b84c4-126">Request body</span></span>
<span data-ttu-id="b84c4-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b84c4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b84c4-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b84c4-128">Response</span></span>
<span data-ttu-id="b84c4-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b84c4-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b84c4-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b84c4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b84c4-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b84c4-131">Request</span></span>
<span data-ttu-id="b84c4-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b84c4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="b84c4-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b84c4-133">Response</span></span>
<span data-ttu-id="b84c4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b84c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 889

{
  "value": [
    {
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
  ]
}
```




