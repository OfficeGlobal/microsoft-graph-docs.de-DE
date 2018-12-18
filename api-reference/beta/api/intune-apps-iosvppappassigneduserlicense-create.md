---
title: Erstellen von iosVppAppAssignedUserLicense
description: Erstellen eines neuen IosVppAppAssignedUserLicense-Objekts.
author: tfitzmac
ms.openlocfilehash: 93b92d28a73e253eb598d03d3171318d95d3fd8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308981"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="ed69e-103">Erstellen von iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="ed69e-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="ed69e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed69e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed69e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed69e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed69e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ed69e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed69e-107">Erstellen eines neuen [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ed69e-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed69e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ed69e-108">Prerequisites</span></span>
<span data-ttu-id="ed69e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed69e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed69e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed69e-111">Permission type</span></span>|<span data-ttu-id="ed69e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed69e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed69e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed69e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed69e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed69e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ed69e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed69e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed69e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed69e-116">Not supported.</span></span>|
|<span data-ttu-id="ed69e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed69e-117">Application</span></span>|<span data-ttu-id="ed69e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed69e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed69e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed69e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="ed69e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed69e-120">Request headers</span></span>
|<span data-ttu-id="ed69e-121">Header</span><span class="sxs-lookup"><span data-stu-id="ed69e-121">Header</span></span>|<span data-ttu-id="ed69e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ed69e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed69e-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ed69e-123">Authorization</span></span>|<span data-ttu-id="ed69e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ed69e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed69e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ed69e-125">Accept</span></span>|<span data-ttu-id="ed69e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ed69e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed69e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed69e-127">Request body</span></span>
<span data-ttu-id="ed69e-128">Geben Sie im Textkörper Anforderung für das Objekt IosVppAppAssignedUserLicense eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ed69e-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="ed69e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosVppAppAssignedUserLicense erstellen.</span><span class="sxs-lookup"><span data-stu-id="ed69e-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="ed69e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed69e-130">Property</span></span>|<span data-ttu-id="ed69e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ed69e-131">Type</span></span>|<span data-ttu-id="ed69e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed69e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed69e-133">id</span><span class="sxs-lookup"><span data-stu-id="ed69e-133">id</span></span>|<span data-ttu-id="ed69e-134">String</span><span class="sxs-lookup"><span data-stu-id="ed69e-134">String</span></span>|<span data-ttu-id="ed69e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ed69e-135">Key of the entity.</span></span> <span data-ttu-id="ed69e-136">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ed69e-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ed69e-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ed69e-137">userEmailAddress</span></span>|<span data-ttu-id="ed69e-138">String</span><span class="sxs-lookup"><span data-stu-id="ed69e-138">String</span></span>|<span data-ttu-id="ed69e-139">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="ed69e-139">The user email address.</span></span> <span data-ttu-id="ed69e-140">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ed69e-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ed69e-141">userId</span><span class="sxs-lookup"><span data-stu-id="ed69e-141">userId</span></span>|<span data-ttu-id="ed69e-142">String</span><span class="sxs-lookup"><span data-stu-id="ed69e-142">String</span></span>|<span data-ttu-id="ed69e-143">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="ed69e-143">The user ID.</span></span> <span data-ttu-id="ed69e-144">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ed69e-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ed69e-145">userName</span><span class="sxs-lookup"><span data-stu-id="ed69e-145">userName</span></span>|<span data-ttu-id="ed69e-146">String</span><span class="sxs-lookup"><span data-stu-id="ed69e-146">String</span></span>|<span data-ttu-id="ed69e-147">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="ed69e-147">The user name.</span></span> <span data-ttu-id="ed69e-148">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ed69e-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="ed69e-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed69e-149">userPrincipalName</span></span>|<span data-ttu-id="ed69e-150">String</span><span class="sxs-lookup"><span data-stu-id="ed69e-150">String</span></span>|<span data-ttu-id="ed69e-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="ed69e-151">The user principal name.</span></span> <span data-ttu-id="ed69e-152">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="ed69e-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ed69e-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed69e-153">Response</span></span>
<span data-ttu-id="ed69e-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ed69e-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed69e-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed69e-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed69e-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed69e-156">Request</span></span>
<span data-ttu-id="ed69e-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed69e-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="ed69e-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed69e-158">Response</span></span>
<span data-ttu-id="ed69e-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed69e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





