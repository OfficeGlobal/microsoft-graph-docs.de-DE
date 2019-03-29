---
title: IosVppAppAssignedUserLicense erstellen
description: Erstellen eines neuen iosVppAppAssignedUserLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e905316197453dfde89f8e074a8105b88d28e1c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970450"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="20ee8-103">IosVppAppAssignedUserLicense erstellen</span><span class="sxs-lookup"><span data-stu-id="20ee8-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="20ee8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20ee8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20ee8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="20ee8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20ee8-106">Erstellen eines neuen [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="20ee8-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20ee8-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="20ee8-107">Prerequisites</span></span>
<span data-ttu-id="20ee8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20ee8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20ee8-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="20ee8-110">Permission type</span></span>|<span data-ttu-id="20ee8-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20ee8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20ee8-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20ee8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20ee8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20ee8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20ee8-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20ee8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20ee8-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20ee8-115">Not supported.</span></span>|
|<span data-ttu-id="20ee8-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20ee8-116">Application</span></span>|<span data-ttu-id="20ee8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20ee8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20ee8-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20ee8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="20ee8-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20ee8-119">Request headers</span></span>
|<span data-ttu-id="20ee8-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="20ee8-120">Header</span></span>|<span data-ttu-id="20ee8-121">Wert</span><span class="sxs-lookup"><span data-stu-id="20ee8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20ee8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20ee8-122">Authorization</span></span>|<span data-ttu-id="20ee8-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="20ee8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20ee8-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="20ee8-124">Accept</span></span>|<span data-ttu-id="20ee8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20ee8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20ee8-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20ee8-126">Request body</span></span>
<span data-ttu-id="20ee8-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das iosVppAppAssignedUserLicense-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="20ee8-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="20ee8-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppAppAssignedUserLicense erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="20ee8-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="20ee8-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20ee8-129">Property</span></span>|<span data-ttu-id="20ee8-130">Typ</span><span class="sxs-lookup"><span data-stu-id="20ee8-130">Type</span></span>|<span data-ttu-id="20ee8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20ee8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20ee8-132">id</span><span class="sxs-lookup"><span data-stu-id="20ee8-132">id</span></span>|<span data-ttu-id="20ee8-133">String</span><span class="sxs-lookup"><span data-stu-id="20ee8-133">String</span></span>|<span data-ttu-id="20ee8-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="20ee8-134">Key of the entity.</span></span> <span data-ttu-id="20ee8-135">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="20ee8-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="20ee8-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="20ee8-136">userEmailAddress</span></span>|<span data-ttu-id="20ee8-137">String</span><span class="sxs-lookup"><span data-stu-id="20ee8-137">String</span></span>|<span data-ttu-id="20ee8-138">Die Benutzer-e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="20ee8-138">The user email address.</span></span> <span data-ttu-id="20ee8-139">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="20ee8-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="20ee8-140">userId</span><span class="sxs-lookup"><span data-stu-id="20ee8-140">userId</span></span>|<span data-ttu-id="20ee8-141">String</span><span class="sxs-lookup"><span data-stu-id="20ee8-141">String</span></span>|<span data-ttu-id="20ee8-142">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="20ee8-142">The user ID.</span></span> <span data-ttu-id="20ee8-143">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="20ee8-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="20ee8-144">userName</span><span class="sxs-lookup"><span data-stu-id="20ee8-144">userName</span></span>|<span data-ttu-id="20ee8-145">String</span><span class="sxs-lookup"><span data-stu-id="20ee8-145">String</span></span>|<span data-ttu-id="20ee8-146">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="20ee8-146">The user name.</span></span> <span data-ttu-id="20ee8-147">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="20ee8-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="20ee8-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="20ee8-148">userPrincipalName</span></span>|<span data-ttu-id="20ee8-149">String</span><span class="sxs-lookup"><span data-stu-id="20ee8-149">String</span></span>|<span data-ttu-id="20ee8-150">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="20ee8-150">The user principal name.</span></span> <span data-ttu-id="20ee8-151">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="20ee8-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="20ee8-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="20ee8-152">Response</span></span>
<span data-ttu-id="20ee8-153">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="20ee8-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20ee8-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="20ee8-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="20ee8-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="20ee8-155">Request</span></span>
<span data-ttu-id="20ee8-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="20ee8-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20ee8-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="20ee8-157">Response</span></span>
<span data-ttu-id="20ee8-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20ee8-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




