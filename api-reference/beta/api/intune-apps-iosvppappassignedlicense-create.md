---
title: IosVppAppAssignedLicense erstellen
description: Erstellen eines neuen iosVppAppAssignedLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eff71bebc59285d5938d784bc57249772d225d95
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154810"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="33f0d-103">IosVppAppAssignedLicense erstellen</span><span class="sxs-lookup"><span data-stu-id="33f0d-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="33f0d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="33f0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33f0d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="33f0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33f0d-106">Erstellen eines neuen [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="33f0d-106">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33f0d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="33f0d-107">Prerequisites</span></span>
<span data-ttu-id="33f0d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="33f0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="33f0d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="33f0d-110">Permission type</span></span>|<span data-ttu-id="33f0d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="33f0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33f0d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="33f0d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33f0d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33f0d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="33f0d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="33f0d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33f0d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33f0d-115">Not supported.</span></span>|
|<span data-ttu-id="33f0d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="33f0d-116">Application</span></span>|<span data-ttu-id="33f0d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="33f0d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33f0d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="33f0d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="33f0d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="33f0d-119">Request headers</span></span>
|<span data-ttu-id="33f0d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="33f0d-120">Header</span></span>|<span data-ttu-id="33f0d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="33f0d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33f0d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="33f0d-122">Authorization</span></span>|<span data-ttu-id="33f0d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="33f0d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33f0d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="33f0d-124">Accept</span></span>|<span data-ttu-id="33f0d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="33f0d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33f0d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="33f0d-126">Request body</span></span>
<span data-ttu-id="33f0d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das iosVppAppAssignedLicense-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="33f0d-127">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="33f0d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppAppAssignedLicense erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="33f0d-128">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="33f0d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="33f0d-129">Property</span></span>|<span data-ttu-id="33f0d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="33f0d-130">Type</span></span>|<span data-ttu-id="33f0d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="33f0d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33f0d-132">id</span><span class="sxs-lookup"><span data-stu-id="33f0d-132">id</span></span>|<span data-ttu-id="33f0d-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33f0d-133">String</span></span>|<span data-ttu-id="33f0d-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="33f0d-134">Key of the entity.</span></span>|
|<span data-ttu-id="33f0d-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="33f0d-135">userEmailAddress</span></span>|<span data-ttu-id="33f0d-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33f0d-136">String</span></span>|<span data-ttu-id="33f0d-137">Die Benutzer-e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="33f0d-137">The user email address.</span></span>|
|<span data-ttu-id="33f0d-138">userId</span><span class="sxs-lookup"><span data-stu-id="33f0d-138">userId</span></span>|<span data-ttu-id="33f0d-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33f0d-139">String</span></span>|<span data-ttu-id="33f0d-140">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="33f0d-140">The user ID.</span></span>|
|<span data-ttu-id="33f0d-141">userName</span><span class="sxs-lookup"><span data-stu-id="33f0d-141">userName</span></span>|<span data-ttu-id="33f0d-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33f0d-142">String</span></span>|<span data-ttu-id="33f0d-143">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="33f0d-143">The user name.</span></span>|
|<span data-ttu-id="33f0d-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="33f0d-144">userPrincipalName</span></span>|<span data-ttu-id="33f0d-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="33f0d-145">String</span></span>|<span data-ttu-id="33f0d-146">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="33f0d-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="33f0d-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="33f0d-147">Response</span></span>
<span data-ttu-id="33f0d-148">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="33f0d-148">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33f0d-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33f0d-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="33f0d-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33f0d-150">Request</span></span>
<span data-ttu-id="33f0d-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33f0d-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="33f0d-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="33f0d-152">Response</span></span>
<span data-ttu-id="33f0d-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33f0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 283

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




