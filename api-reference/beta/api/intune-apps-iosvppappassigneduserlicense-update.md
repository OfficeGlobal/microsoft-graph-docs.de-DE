---
title: IosVppAppAssignedUserLicense aktualisieren
description: Aktualisieren der Eigenschaften eines iosVppAppAssignedUserLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee92728dbf1570bf44f311007b92f80af6fe9c44
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974713"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="c99c1-103">IosVppAppAssignedUserLicense aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c99c1-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="c99c1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c99c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c99c1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c99c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c99c1-106">Aktualisieren der Eigenschaften eines [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c99c1-106">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c99c1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c99c1-107">Prerequisites</span></span>
<span data-ttu-id="c99c1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c99c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c99c1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c99c1-110">Permission type</span></span>|<span data-ttu-id="c99c1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c99c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c99c1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c99c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c99c1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c99c1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c99c1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c99c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c99c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c99c1-115">Not supported.</span></span>|
|<span data-ttu-id="c99c1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c99c1-116">Application</span></span>|<span data-ttu-id="c99c1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c99c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c99c1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c99c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="c99c1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c99c1-119">Request headers</span></span>
|<span data-ttu-id="c99c1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c99c1-120">Header</span></span>|<span data-ttu-id="c99c1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c99c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c99c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c99c1-122">Authorization</span></span>|<span data-ttu-id="c99c1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c99c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c99c1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c99c1-124">Accept</span></span>|<span data-ttu-id="c99c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c99c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c99c1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c99c1-126">Request body</span></span>
<span data-ttu-id="c99c1-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c99c1-127">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="c99c1-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c99c1-128">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="c99c1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c99c1-129">Property</span></span>|<span data-ttu-id="c99c1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c99c1-130">Type</span></span>|<span data-ttu-id="c99c1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c99c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c99c1-132">id</span><span class="sxs-lookup"><span data-stu-id="c99c1-132">id</span></span>|<span data-ttu-id="c99c1-133">String</span><span class="sxs-lookup"><span data-stu-id="c99c1-133">String</span></span>|<span data-ttu-id="c99c1-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c99c1-134">Key of the entity.</span></span> <span data-ttu-id="c99c1-135">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c99c1-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c99c1-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c99c1-136">userEmailAddress</span></span>|<span data-ttu-id="c99c1-137">String</span><span class="sxs-lookup"><span data-stu-id="c99c1-137">String</span></span>|<span data-ttu-id="c99c1-138">Die Benutzer-e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="c99c1-138">The user email address.</span></span> <span data-ttu-id="c99c1-139">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c99c1-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c99c1-140">userId</span><span class="sxs-lookup"><span data-stu-id="c99c1-140">userId</span></span>|<span data-ttu-id="c99c1-141">String</span><span class="sxs-lookup"><span data-stu-id="c99c1-141">String</span></span>|<span data-ttu-id="c99c1-142">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="c99c1-142">The user ID.</span></span> <span data-ttu-id="c99c1-143">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c99c1-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c99c1-144">userName</span><span class="sxs-lookup"><span data-stu-id="c99c1-144">userName</span></span>|<span data-ttu-id="c99c1-145">String</span><span class="sxs-lookup"><span data-stu-id="c99c1-145">String</span></span>|<span data-ttu-id="c99c1-146">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="c99c1-146">The user name.</span></span> <span data-ttu-id="c99c1-147">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c99c1-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c99c1-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c99c1-148">userPrincipalName</span></span>|<span data-ttu-id="c99c1-149">String</span><span class="sxs-lookup"><span data-stu-id="c99c1-149">String</span></span>|<span data-ttu-id="c99c1-150">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="c99c1-150">The user principal name.</span></span> <span data-ttu-id="c99c1-151">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c99c1-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c99c1-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="c99c1-152">Response</span></span>
<span data-ttu-id="c99c1-153">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c99c1-153">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c99c1-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c99c1-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c99c1-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c99c1-155">Request</span></span>
<span data-ttu-id="c99c1-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c99c1-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="c99c1-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="c99c1-157">Response</span></span>
<span data-ttu-id="c99c1-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c99c1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




