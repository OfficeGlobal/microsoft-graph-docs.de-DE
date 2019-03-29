---
title: IosVppAppAssignedLicense erstellen
description: Erstellen eines neuen iosVppAppAssignedLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2014cde4b446f3a629ef0f99485a081eb7909384
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974573"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="2e3cd-103">IosVppAppAssignedLicense erstellen</span><span class="sxs-lookup"><span data-stu-id="2e3cd-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="2e3cd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e3cd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e3cd-106">Erstellen eines neuen [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-106">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e3cd-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2e3cd-107">Prerequisites</span></span>
<span data-ttu-id="2e3cd-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e3cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e3cd-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e3cd-110">Permission type</span></span>|<span data-ttu-id="2e3cd-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e3cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e3cd-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e3cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2e3cd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e3cd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e3cd-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e3cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e3cd-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e3cd-115">Not supported.</span></span>|
|<span data-ttu-id="2e3cd-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e3cd-116">Application</span></span>|<span data-ttu-id="2e3cd-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e3cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e3cd-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e3cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="2e3cd-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e3cd-119">Request headers</span></span>
|<span data-ttu-id="2e3cd-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2e3cd-120">Header</span></span>|<span data-ttu-id="2e3cd-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2e3cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e3cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e3cd-122">Authorization</span></span>|<span data-ttu-id="2e3cd-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2e3cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e3cd-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2e3cd-124">Accept</span></span>|<span data-ttu-id="2e3cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e3cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e3cd-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e3cd-126">Request body</span></span>
<span data-ttu-id="2e3cd-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das iosVppAppAssignedLicense-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-127">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="2e3cd-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der iosVppAppAssignedLicense erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-128">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="2e3cd-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e3cd-129">Property</span></span>|<span data-ttu-id="2e3cd-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2e3cd-130">Type</span></span>|<span data-ttu-id="2e3cd-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e3cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e3cd-132">id</span><span class="sxs-lookup"><span data-stu-id="2e3cd-132">id</span></span>|<span data-ttu-id="2e3cd-133">String</span><span class="sxs-lookup"><span data-stu-id="2e3cd-133">String</span></span>|<span data-ttu-id="2e3cd-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2e3cd-134">Key of the entity.</span></span>|
|<span data-ttu-id="2e3cd-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2e3cd-135">userEmailAddress</span></span>|<span data-ttu-id="2e3cd-136">String</span><span class="sxs-lookup"><span data-stu-id="2e3cd-136">String</span></span>|<span data-ttu-id="2e3cd-137">Die Benutzer-e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-137">The user email address.</span></span>|
|<span data-ttu-id="2e3cd-138">userId</span><span class="sxs-lookup"><span data-stu-id="2e3cd-138">userId</span></span>|<span data-ttu-id="2e3cd-139">String</span><span class="sxs-lookup"><span data-stu-id="2e3cd-139">String</span></span>|<span data-ttu-id="2e3cd-140">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-140">The user ID.</span></span>|
|<span data-ttu-id="2e3cd-141">userName</span><span class="sxs-lookup"><span data-stu-id="2e3cd-141">userName</span></span>|<span data-ttu-id="2e3cd-142">String</span><span class="sxs-lookup"><span data-stu-id="2e3cd-142">String</span></span>|<span data-ttu-id="2e3cd-143">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-143">The user name.</span></span>|
|<span data-ttu-id="2e3cd-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e3cd-144">userPrincipalName</span></span>|<span data-ttu-id="2e3cd-145">String</span><span class="sxs-lookup"><span data-stu-id="2e3cd-145">String</span></span>|<span data-ttu-id="2e3cd-146">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="2e3cd-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e3cd-147">Response</span></span>
<span data-ttu-id="2e3cd-148">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-148">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e3cd-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e3cd-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e3cd-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e3cd-150">Request</span></span>
<span data-ttu-id="2e3cd-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2e3cd-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e3cd-152">Response</span></span>
<span data-ttu-id="2e3cd-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e3cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




