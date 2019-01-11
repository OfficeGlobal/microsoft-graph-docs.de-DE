---
title: Erstellen von iosVppAppAssignedLicense
description: Erstellen eines neuen IosVppAppAssignedLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 225b7168d584faa2e5ff1ec2910fe0e3e53fda8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887101"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="8911d-103">Erstellen von iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="8911d-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="8911d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8911d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8911d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8911d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8911d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8911d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8911d-107">Erstellen eines neuen [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="8911d-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8911d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8911d-108">Prerequisites</span></span>
<span data-ttu-id="8911d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8911d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8911d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8911d-111">Permission type</span></span>|<span data-ttu-id="8911d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8911d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8911d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8911d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8911d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8911d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8911d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8911d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8911d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8911d-116">Not supported.</span></span>|
|<span data-ttu-id="8911d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8911d-117">Application</span></span>|<span data-ttu-id="8911d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8911d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8911d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8911d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="8911d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8911d-120">Request headers</span></span>
|<span data-ttu-id="8911d-121">Header</span><span class="sxs-lookup"><span data-stu-id="8911d-121">Header</span></span>|<span data-ttu-id="8911d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8911d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8911d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8911d-123">Authorization</span></span>|<span data-ttu-id="8911d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8911d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8911d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="8911d-125">Accept</span></span>|<span data-ttu-id="8911d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8911d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8911d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8911d-127">Request body</span></span>
<span data-ttu-id="8911d-128">Geben Sie im Textkörper Anforderung für das Objekt IosVppAppAssignedLicense eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="8911d-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="8911d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die IosVppAppAssignedLicense erstellen.</span><span class="sxs-lookup"><span data-stu-id="8911d-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="8911d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8911d-130">Property</span></span>|<span data-ttu-id="8911d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8911d-131">Type</span></span>|<span data-ttu-id="8911d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8911d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8911d-133">id</span><span class="sxs-lookup"><span data-stu-id="8911d-133">id</span></span>|<span data-ttu-id="8911d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8911d-134">String</span></span>|<span data-ttu-id="8911d-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8911d-135">Key of the entity.</span></span>|
|<span data-ttu-id="8911d-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8911d-136">userEmailAddress</span></span>|<span data-ttu-id="8911d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8911d-137">String</span></span>|<span data-ttu-id="8911d-138">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="8911d-138">The user email address.</span></span>|
|<span data-ttu-id="8911d-139">userId</span><span class="sxs-lookup"><span data-stu-id="8911d-139">userId</span></span>|<span data-ttu-id="8911d-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8911d-140">String</span></span>|<span data-ttu-id="8911d-141">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="8911d-141">The user ID.</span></span>|
|<span data-ttu-id="8911d-142">userName</span><span class="sxs-lookup"><span data-stu-id="8911d-142">userName</span></span>|<span data-ttu-id="8911d-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8911d-143">String</span></span>|<span data-ttu-id="8911d-144">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="8911d-144">The user name.</span></span>|
|<span data-ttu-id="8911d-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8911d-145">userPrincipalName</span></span>|<span data-ttu-id="8911d-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8911d-146">String</span></span>|<span data-ttu-id="8911d-147">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="8911d-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="8911d-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="8911d-148">Response</span></span>
<span data-ttu-id="8911d-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="8911d-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8911d-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8911d-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="8911d-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8911d-151">Request</span></span>
<span data-ttu-id="8911d-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8911d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8911d-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="8911d-153">Response</span></span>
<span data-ttu-id="8911d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8911d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





