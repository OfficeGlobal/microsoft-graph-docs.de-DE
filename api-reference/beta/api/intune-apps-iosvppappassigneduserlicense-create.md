---
title: Erstellen von iosVppAppAssignedUserLicense
description: Erstellen eines neuen IosVppAppAssignedUserLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2e6178570da6e89ef50c933d027daa2a9d7e1adf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864652"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="4d051-103">Erstellen von iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="4d051-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="4d051-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4d051-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d051-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d051-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d051-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4d051-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d051-107">Erstellen eines neuen [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="4d051-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d051-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d051-108">Prerequisites</span></span>
<span data-ttu-id="4d051-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d051-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d051-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d051-111">Permission type</span></span>|<span data-ttu-id="4d051-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d051-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d051-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d051-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d051-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d051-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4d051-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d051-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d051-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d051-116">Not supported.</span></span>|
|<span data-ttu-id="4d051-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d051-117">Application</span></span>|<span data-ttu-id="4d051-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d051-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d051-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d051-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="4d051-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d051-120">Request headers</span></span>
|<span data-ttu-id="4d051-121">Header</span><span class="sxs-lookup"><span data-stu-id="4d051-121">Header</span></span>|<span data-ttu-id="4d051-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4d051-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d051-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d051-123">Authorization</span></span>|<span data-ttu-id="4d051-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d051-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d051-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4d051-125">Accept</span></span>|<span data-ttu-id="4d051-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d051-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d051-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d051-127">Request body</span></span>
<span data-ttu-id="4d051-128">Geben Sie im Textkörper Anforderung für das Objekt IosVppAppAssignedUserLicense eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="4d051-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="4d051-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosVppAppAssignedUserLicense erstellen.</span><span class="sxs-lookup"><span data-stu-id="4d051-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="4d051-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d051-130">Property</span></span>|<span data-ttu-id="4d051-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4d051-131">Type</span></span>|<span data-ttu-id="4d051-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d051-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d051-133">id</span><span class="sxs-lookup"><span data-stu-id="4d051-133">id</span></span>|<span data-ttu-id="4d051-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d051-134">String</span></span>|<span data-ttu-id="4d051-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4d051-135">Key of the entity.</span></span> <span data-ttu-id="4d051-136">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4d051-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="4d051-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="4d051-137">userEmailAddress</span></span>|<span data-ttu-id="4d051-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d051-138">String</span></span>|<span data-ttu-id="4d051-139">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4d051-139">The user email address.</span></span> <span data-ttu-id="4d051-140">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4d051-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="4d051-141">userId</span><span class="sxs-lookup"><span data-stu-id="4d051-141">userId</span></span>|<span data-ttu-id="4d051-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d051-142">String</span></span>|<span data-ttu-id="4d051-143">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="4d051-143">The user ID.</span></span> <span data-ttu-id="4d051-144">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4d051-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="4d051-145">userName</span><span class="sxs-lookup"><span data-stu-id="4d051-145">userName</span></span>|<span data-ttu-id="4d051-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d051-146">String</span></span>|<span data-ttu-id="4d051-147">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="4d051-147">The user name.</span></span> <span data-ttu-id="4d051-148">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4d051-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="4d051-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4d051-149">userPrincipalName</span></span>|<span data-ttu-id="4d051-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d051-150">String</span></span>|<span data-ttu-id="4d051-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="4d051-151">The user principal name.</span></span> <span data-ttu-id="4d051-152">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="4d051-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4d051-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d051-153">Response</span></span>
<span data-ttu-id="4d051-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4d051-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d051-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d051-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d051-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d051-156">Request</span></span>
<span data-ttu-id="4d051-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d051-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4d051-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d051-158">Response</span></span>
<span data-ttu-id="4d051-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d051-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





