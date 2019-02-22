---
title: MacOsVppAppAssignedLicense löschen
description: Löscht eine macOsVppAppAssignedLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad416daa9619381f882eabb3a0f7c251ad471567
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153060"
---
# <a name="delete-macosvppappassignedlicense"></a><span data-ttu-id="f9332-103">MacOsVppAppAssignedLicense löschen</span><span class="sxs-lookup"><span data-stu-id="f9332-103">Delete macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="f9332-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9332-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9332-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f9332-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9332-106">Löscht eine [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="f9332-106">Deletes a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9332-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f9332-107">Prerequisites</span></span>
<span data-ttu-id="f9332-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f9332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f9332-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f9332-110">Permission type</span></span>|<span data-ttu-id="f9332-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f9332-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9332-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f9332-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9332-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9332-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9332-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f9332-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9332-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9332-115">Not supported.</span></span>|
|<span data-ttu-id="f9332-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f9332-116">Application</span></span>|<span data-ttu-id="f9332-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f9332-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9332-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9332-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="f9332-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f9332-119">Request headers</span></span>
|<span data-ttu-id="f9332-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f9332-120">Header</span></span>|<span data-ttu-id="f9332-121">Wert</span><span class="sxs-lookup"><span data-stu-id="f9332-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9332-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9332-122">Authorization</span></span>|<span data-ttu-id="f9332-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f9332-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9332-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f9332-124">Accept</span></span>|<span data-ttu-id="f9332-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9332-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9332-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f9332-126">Request body</span></span>
<span data-ttu-id="f9332-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f9332-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9332-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9332-128">Response</span></span>
<span data-ttu-id="f9332-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9332-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f9332-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f9332-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9332-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f9332-131">Request</span></span>
<span data-ttu-id="f9332-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f9332-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="f9332-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f9332-133">Response</span></span>
<span data-ttu-id="f9332-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f9332-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




