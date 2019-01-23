---
title: GetTopMobileApps-Funktion
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f29c6dfe6502b1520e2100781d47688bbbe5d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417028"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="6d133-103">GetTopMobileApps-Funktion</span><span class="sxs-lookup"><span data-stu-id="6d133-103">getTopMobileApps function</span></span>

> <span data-ttu-id="6d133-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6d133-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6d133-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6d133-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d133-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6d133-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d133-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6d133-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d133-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6d133-108">Prerequisites</span></span>
<span data-ttu-id="6d133-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d133-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6d133-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6d133-111">Permission type</span></span>|<span data-ttu-id="6d133-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6d133-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d133-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6d133-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d133-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d133-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6d133-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6d133-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d133-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d133-116">Not supported.</span></span>|
|<span data-ttu-id="6d133-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6d133-117">Application</span></span>|<span data-ttu-id="6d133-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6d133-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d133-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d133-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6d133-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6d133-120">Request headers</span></span>
|<span data-ttu-id="6d133-121">Header</span><span class="sxs-lookup"><span data-stu-id="6d133-121">Header</span></span>|<span data-ttu-id="6d133-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6d133-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d133-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="6d133-123">Authorization</span></span>|<span data-ttu-id="6d133-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6d133-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d133-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6d133-125">Accept</span></span>|<span data-ttu-id="6d133-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d133-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d133-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6d133-127">Request body</span></span>
<span data-ttu-id="6d133-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="6d133-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="6d133-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="6d133-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="6d133-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6d133-130">Property</span></span>|<span data-ttu-id="6d133-131">Typ</span><span class="sxs-lookup"><span data-stu-id="6d133-131">Type</span></span>|<span data-ttu-id="6d133-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6d133-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d133-133">status</span><span class="sxs-lookup"><span data-stu-id="6d133-133">status</span></span>|<span data-ttu-id="6d133-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6d133-134">String</span></span>|<span data-ttu-id="6d133-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6d133-135">Not yet documented</span></span>|
|<span data-ttu-id="6d133-136">count</span><span class="sxs-lookup"><span data-stu-id="6d133-136">count</span></span>|<span data-ttu-id="6d133-137">Int64</span><span class="sxs-lookup"><span data-stu-id="6d133-137">Int64</span></span>|<span data-ttu-id="6d133-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6d133-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6d133-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d133-139">Response</span></span>
<span data-ttu-id="6d133-140">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [MobileApp](../resources/intune-apps-mobileapp.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="6d133-140">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d133-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6d133-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d133-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6d133-142">Request</span></span>
<span data-ttu-id="6d133-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6d133-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="6d133-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="6d133-144">Response</span></span>
<span data-ttu-id="6d133-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6d133-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 982

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
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
      ]
    }
  ]
}
```




