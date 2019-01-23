---
title: targetedManagedAppConfiguration abrufen
description: Lesen von Eigenschaften und Beziehungen des targetedManagedAppConfiguration-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2deff854e237c221aaf8610d43bed761477a6251
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420234"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="e74ea-103">targetedManagedAppConfiguration abrufen</span><span class="sxs-lookup"><span data-stu-id="e74ea-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="e74ea-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e74ea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e74ea-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e74ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e74ea-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e74ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e74ea-107">Lesen von Eigenschaften und Beziehungen des [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e74ea-107">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e74ea-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e74ea-108">Prerequisites</span></span>
<span data-ttu-id="e74ea-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e74ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e74ea-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e74ea-111">Permission type</span></span>|<span data-ttu-id="e74ea-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e74ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e74ea-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e74ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e74ea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e74ea-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e74ea-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e74ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e74ea-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e74ea-116">Not supported.</span></span>|
|<span data-ttu-id="e74ea-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e74ea-117">Application</span></span>|<span data-ttu-id="e74ea-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e74ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e74ea-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e74ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e74ea-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e74ea-120">Optional query parameters</span></span>
<span data-ttu-id="e74ea-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e74ea-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e74ea-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e74ea-122">Request headers</span></span>
|<span data-ttu-id="e74ea-123">Header</span><span class="sxs-lookup"><span data-stu-id="e74ea-123">Header</span></span>|<span data-ttu-id="e74ea-124">Wert</span><span class="sxs-lookup"><span data-stu-id="e74ea-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e74ea-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="e74ea-125">Authorization</span></span>|<span data-ttu-id="e74ea-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e74ea-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e74ea-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e74ea-127">Accept</span></span>|<span data-ttu-id="e74ea-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e74ea-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e74ea-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e74ea-129">Request body</span></span>
<span data-ttu-id="e74ea-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e74ea-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e74ea-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e74ea-131">Response</span></span>
<span data-ttu-id="e74ea-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e74ea-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e74ea-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e74ea-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e74ea-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e74ea-134">Request</span></span>
<span data-ttu-id="e74ea-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e74ea-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e74ea-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e74ea-136">Response</span></span>
<span data-ttu-id="e74ea-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e74ea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 679

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
}
```




