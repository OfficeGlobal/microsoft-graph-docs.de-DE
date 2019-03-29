---
title: AndroidManagedStoreApps aufListen
description: AufListen von Eigenschaften und Beziehungen der androidManagedStoreApp-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efd5be62e0c55b467042c21f380d3fe5792a9b98
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982945"
---
# <a name="list-androidmanagedstoreapps"></a><span data-ttu-id="f46c3-103">AndroidManagedStoreApps aufListen</span><span class="sxs-lookup"><span data-stu-id="f46c3-103">List androidManagedStoreApps</span></span>

> <span data-ttu-id="f46c3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f46c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f46c3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f46c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f46c3-106">AufListen von Eigenschaften und Beziehungen der [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="f46c3-106">List properties and relationships of the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f46c3-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f46c3-107">Prerequisites</span></span>
<span data-ttu-id="f46c3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f46c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f46c3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f46c3-110">Permission type</span></span>|<span data-ttu-id="f46c3-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f46c3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f46c3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f46c3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f46c3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f46c3-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f46c3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f46c3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f46c3-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f46c3-115">Not supported.</span></span>|
|<span data-ttu-id="f46c3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f46c3-116">Application</span></span>|<span data-ttu-id="f46c3-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f46c3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f46c3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f46c3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f46c3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f46c3-119">Request headers</span></span>
|<span data-ttu-id="f46c3-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f46c3-120">Header</span></span>|<span data-ttu-id="f46c3-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f46c3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f46c3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f46c3-122">Authorization</span></span>|<span data-ttu-id="f46c3-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f46c3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f46c3-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f46c3-124">Accept</span></span>|<span data-ttu-id="f46c3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f46c3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f46c3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f46c3-126">Request body</span></span>
<span data-ttu-id="f46c3-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f46c3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f46c3-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f46c3-128">Response</span></span>
<span data-ttu-id="f46c3-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f46c3-129">If successful, this method returns a `200 OK` response code and a collection of [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f46c3-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f46c3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f46c3-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f46c3-131">Request</span></span>
<span data-ttu-id="f46c3-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f46c3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="f46c3-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f46c3-133">Response</span></span>
<span data-ttu-id="f46c3-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f46c3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1236

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreApp",
      "id": "87247525-7525-8724-2575-248725752487",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
      "usedLicenseCount": 0,
      "totalLicenseCount": 1,
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "supportsOemConfig": true
    }
  ]
}
```




