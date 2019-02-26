---
title: IosVppAppAssignedUserLicense erstellen
description: Erstellen eines neuen iosVppAppAssignedUserLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f1efba3659190080c507ca3418bacd9bc7d6461
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157526"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="6c86c-103">IosVppAppAssignedUserLicense erstellen</span><span class="sxs-lookup"><span data-stu-id="6c86c-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="6c86c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6c86c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c86c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6c86c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c86c-106">Erstellen eines neuen [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c86c-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c86c-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6c86c-107">Prerequisites</span></span>
<span data-ttu-id="6c86c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6c86c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6c86c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c86c-110">Permission type</span></span>|<span data-ttu-id="6c86c-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c86c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c86c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c86c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c86c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c86c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c86c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c86c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c86c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c86c-115">Not supported.</span></span>|
|<span data-ttu-id="6c86c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c86c-116">Application</span></span>|<span data-ttu-id="6c86c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6c86c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c86c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c86c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="6c86c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c86c-119">Request headers</span></span>
|<span data-ttu-id="6c86c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6c86c-120">Header</span></span>|<span data-ttu-id="6c86c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6c86c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c86c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c86c-122">Authorization</span></span>|<span data-ttu-id="6c86c-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6c86c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c86c-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6c86c-124">Accept</span></span>|<span data-ttu-id="6c86c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c86c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c86c-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c86c-126">Request body</span></span>
<span data-ttu-id="6c86c-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das iosVppAppAssignedUserLicense-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="6c86c-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="6c86c-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppAppAssignedUserLicense erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="6c86c-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="6c86c-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6c86c-129">Property</span></span>|<span data-ttu-id="6c86c-130">Typ</span><span class="sxs-lookup"><span data-stu-id="6c86c-130">Type</span></span>|<span data-ttu-id="6c86c-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c86c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c86c-132">id</span><span class="sxs-lookup"><span data-stu-id="6c86c-132">id</span></span>|<span data-ttu-id="6c86c-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c86c-133">String</span></span>|<span data-ttu-id="6c86c-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="6c86c-134">Key of the entity.</span></span> <span data-ttu-id="6c86c-135">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c86c-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="6c86c-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="6c86c-136">userEmailAddress</span></span>|<span data-ttu-id="6c86c-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c86c-137">String</span></span>|<span data-ttu-id="6c86c-138">Die Benutzer-e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="6c86c-138">The user email address.</span></span> <span data-ttu-id="6c86c-139">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c86c-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="6c86c-140">userId</span><span class="sxs-lookup"><span data-stu-id="6c86c-140">userId</span></span>|<span data-ttu-id="6c86c-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c86c-141">String</span></span>|<span data-ttu-id="6c86c-142">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="6c86c-142">The user ID.</span></span> <span data-ttu-id="6c86c-143">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c86c-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="6c86c-144">userName</span><span class="sxs-lookup"><span data-stu-id="6c86c-144">userName</span></span>|<span data-ttu-id="6c86c-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c86c-145">String</span></span>|<span data-ttu-id="6c86c-146">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="6c86c-146">The user name.</span></span> <span data-ttu-id="6c86c-147">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c86c-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="6c86c-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6c86c-148">userPrincipalName</span></span>|<span data-ttu-id="6c86c-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6c86c-149">String</span></span>|<span data-ttu-id="6c86c-150">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="6c86c-150">The user principal name.</span></span> <span data-ttu-id="6c86c-151">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c86c-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6c86c-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c86c-152">Response</span></span>
<span data-ttu-id="6c86c-153">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6c86c-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c86c-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c86c-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c86c-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c86c-155">Request</span></span>
<span data-ttu-id="6c86c-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6c86c-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c86c-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c86c-157">Response</span></span>
<span data-ttu-id="6c86c-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c86c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




