---
title: Abrufen von macOsVppAppAssignedLicense
description: Lesen Sie Eigenschaften und Beziehungen des MacOsVppAppAssignedLicense-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3863359b9f6ab3051b24f22ab4017c5cf29e0316
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430035"
---
# <a name="get-macosvppappassignedlicense"></a><span data-ttu-id="84ebc-103">Abrufen von macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="84ebc-103">Get macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="84ebc-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="84ebc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84ebc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84ebc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84ebc-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="84ebc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ebc-107">Lesen Sie Eigenschaften und Beziehungen des [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="84ebc-107">Read properties and relationships of the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84ebc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84ebc-108">Prerequisites</span></span>
<span data-ttu-id="84ebc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="84ebc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="84ebc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84ebc-111">Permission type</span></span>|<span data-ttu-id="84ebc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84ebc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84ebc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84ebc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84ebc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="84ebc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="84ebc-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84ebc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84ebc-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84ebc-116">Not supported.</span></span>|
|<span data-ttu-id="84ebc-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84ebc-117">Application</span></span>|<span data-ttu-id="84ebc-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84ebc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84ebc-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84ebc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84ebc-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="84ebc-120">Optional query parameters</span></span>
<span data-ttu-id="84ebc-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="84ebc-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84ebc-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84ebc-122">Request headers</span></span>
|<span data-ttu-id="84ebc-123">Header</span><span class="sxs-lookup"><span data-stu-id="84ebc-123">Header</span></span>|<span data-ttu-id="84ebc-124">Wert</span><span class="sxs-lookup"><span data-stu-id="84ebc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84ebc-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="84ebc-125">Authorization</span></span>|<span data-ttu-id="84ebc-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84ebc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84ebc-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="84ebc-127">Accept</span></span>|<span data-ttu-id="84ebc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="84ebc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84ebc-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84ebc-129">Request body</span></span>
<span data-ttu-id="84ebc-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="84ebc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84ebc-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="84ebc-131">Response</span></span>
<span data-ttu-id="84ebc-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="84ebc-132">If successful, this method returns a `200 OK` response code and [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84ebc-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84ebc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="84ebc-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84ebc-134">Request</span></span>
<span data-ttu-id="84ebc-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84ebc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="84ebc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="84ebc-136">Response</span></span>
<span data-ttu-id="84ebc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84ebc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 316

{
  "value": {
    "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
    "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
    "userEmailAddress": "User Email Address value",
    "userId": "User Id value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value"
  }
}
```



