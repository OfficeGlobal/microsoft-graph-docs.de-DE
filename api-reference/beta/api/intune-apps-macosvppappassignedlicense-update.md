---
title: MacOsVppAppAssignedLicense aktualisieren
description: Aktualisieren der Eigenschaften eines macOsVppAppAssignedLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0f0ccb27bb9bedcbd9d83333c60c864dc99e5b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160424"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="ac3ed-103">MacOsVppAppAssignedLicense aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ac3ed-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="ac3ed-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac3ed-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac3ed-106">Aktualisieren der Eigenschaften eines [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-106">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac3ed-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ac3ed-107">Prerequisites</span></span>
<span data-ttu-id="ac3ed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ac3ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ac3ed-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ac3ed-110">Permission type</span></span>|<span data-ttu-id="ac3ed-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ac3ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac3ed-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ac3ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ac3ed-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac3ed-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac3ed-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ac3ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac3ed-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac3ed-115">Not supported.</span></span>|
|<span data-ttu-id="ac3ed-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ac3ed-116">Application</span></span>|<span data-ttu-id="ac3ed-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ac3ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac3ed-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac3ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="ac3ed-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ac3ed-119">Request headers</span></span>
|<span data-ttu-id="ac3ed-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ac3ed-120">Header</span></span>|<span data-ttu-id="ac3ed-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ac3ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac3ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac3ed-122">Authorization</span></span>|<span data-ttu-id="ac3ed-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ac3ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac3ed-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ac3ed-124">Accept</span></span>|<span data-ttu-id="ac3ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ac3ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac3ed-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ac3ed-126">Request body</span></span>
<span data-ttu-id="ac3ed-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-127">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="ac3ed-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-128">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="ac3ed-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ac3ed-129">Property</span></span>|<span data-ttu-id="ac3ed-130">Typ</span><span class="sxs-lookup"><span data-stu-id="ac3ed-130">Type</span></span>|<span data-ttu-id="ac3ed-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ac3ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac3ed-132">id</span><span class="sxs-lookup"><span data-stu-id="ac3ed-132">id</span></span>|<span data-ttu-id="ac3ed-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac3ed-133">String</span></span>|<span data-ttu-id="ac3ed-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ac3ed-134">Key of the entity.</span></span>|
|<span data-ttu-id="ac3ed-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ac3ed-135">userEmailAddress</span></span>|<span data-ttu-id="ac3ed-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac3ed-136">String</span></span>|<span data-ttu-id="ac3ed-137">Die Benutzer-e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-137">The user email address.</span></span>|
|<span data-ttu-id="ac3ed-138">userId</span><span class="sxs-lookup"><span data-stu-id="ac3ed-138">userId</span></span>|<span data-ttu-id="ac3ed-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac3ed-139">String</span></span>|<span data-ttu-id="ac3ed-140">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-140">The user ID.</span></span>|
|<span data-ttu-id="ac3ed-141">userName</span><span class="sxs-lookup"><span data-stu-id="ac3ed-141">userName</span></span>|<span data-ttu-id="ac3ed-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac3ed-142">String</span></span>|<span data-ttu-id="ac3ed-143">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-143">The user name.</span></span>|
|<span data-ttu-id="ac3ed-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ac3ed-144">userPrincipalName</span></span>|<span data-ttu-id="ac3ed-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ac3ed-145">String</span></span>|<span data-ttu-id="ac3ed-146">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="ac3ed-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac3ed-147">Response</span></span>
<span data-ttu-id="ac3ed-148">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-148">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac3ed-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ac3ed-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac3ed-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ac3ed-150">Request</span></span>
<span data-ttu-id="ac3ed-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ac3ed-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="ac3ed-152">Response</span></span>
<span data-ttu-id="ac3ed-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ac3ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




