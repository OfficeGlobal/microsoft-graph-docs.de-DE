---
title: Erstellen von iosVppAppAssignedUserLicense
description: Erstellen eines neuen IosVppAppAssignedUserLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6db9d5cb57ee35d1019722b1d3671a0dd742c5ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919939"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="617c2-103">Erstellen von iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="617c2-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="617c2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="617c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="617c2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="617c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="617c2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="617c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="617c2-107">Erstellen eines neuen [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="617c2-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="617c2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="617c2-108">Prerequisites</span></span>
<span data-ttu-id="617c2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="617c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="617c2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="617c2-111">Permission type</span></span>|<span data-ttu-id="617c2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="617c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="617c2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="617c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="617c2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="617c2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="617c2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="617c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="617c2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="617c2-116">Not supported.</span></span>|
|<span data-ttu-id="617c2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="617c2-117">Application</span></span>|<span data-ttu-id="617c2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="617c2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="617c2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="617c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="617c2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="617c2-120">Request headers</span></span>
|<span data-ttu-id="617c2-121">Header</span><span class="sxs-lookup"><span data-stu-id="617c2-121">Header</span></span>|<span data-ttu-id="617c2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="617c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="617c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="617c2-123">Authorization</span></span>|<span data-ttu-id="617c2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="617c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="617c2-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="617c2-125">Accept</span></span>|<span data-ttu-id="617c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="617c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="617c2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="617c2-127">Request body</span></span>
<span data-ttu-id="617c2-128">Geben Sie im Textkörper Anforderung für das Objekt IosVppAppAssignedUserLicense eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="617c2-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="617c2-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosVppAppAssignedUserLicense erstellen.</span><span class="sxs-lookup"><span data-stu-id="617c2-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="617c2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="617c2-130">Property</span></span>|<span data-ttu-id="617c2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="617c2-131">Type</span></span>|<span data-ttu-id="617c2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="617c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="617c2-133">id</span><span class="sxs-lookup"><span data-stu-id="617c2-133">id</span></span>|<span data-ttu-id="617c2-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="617c2-134">String</span></span>|<span data-ttu-id="617c2-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="617c2-135">Key of the entity.</span></span> <span data-ttu-id="617c2-136">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="617c2-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="617c2-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="617c2-137">userEmailAddress</span></span>|<span data-ttu-id="617c2-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="617c2-138">String</span></span>|<span data-ttu-id="617c2-139">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="617c2-139">The user email address.</span></span> <span data-ttu-id="617c2-140">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="617c2-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="617c2-141">userId</span><span class="sxs-lookup"><span data-stu-id="617c2-141">userId</span></span>|<span data-ttu-id="617c2-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="617c2-142">String</span></span>|<span data-ttu-id="617c2-143">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="617c2-143">The user ID.</span></span> <span data-ttu-id="617c2-144">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="617c2-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="617c2-145">userName</span><span class="sxs-lookup"><span data-stu-id="617c2-145">userName</span></span>|<span data-ttu-id="617c2-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="617c2-146">String</span></span>|<span data-ttu-id="617c2-147">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="617c2-147">The user name.</span></span> <span data-ttu-id="617c2-148">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="617c2-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="617c2-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="617c2-149">userPrincipalName</span></span>|<span data-ttu-id="617c2-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="617c2-150">String</span></span>|<span data-ttu-id="617c2-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="617c2-151">The user principal name.</span></span> <span data-ttu-id="617c2-152">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="617c2-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="617c2-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="617c2-153">Response</span></span>
<span data-ttu-id="617c2-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="617c2-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="617c2-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="617c2-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="617c2-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="617c2-156">Request</span></span>
<span data-ttu-id="617c2-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="617c2-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="617c2-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="617c2-158">Response</span></span>
<span data-ttu-id="617c2-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="617c2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





