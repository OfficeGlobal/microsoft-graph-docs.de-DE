---
title: MacOsVppAppAssignedLicense erstellen
description: Erstellen eines neuen macOsVppAppAssignedLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05424b5f8eaff6f3d055fd6f3babe77fb726b194
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983848"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="726a9-103">MacOsVppAppAssignedLicense erstellen</span><span class="sxs-lookup"><span data-stu-id="726a9-103">Create macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="726a9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="726a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="726a9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="726a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="726a9-106">Erstellen eines neuen [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="726a9-106">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="726a9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="726a9-107">Prerequisites</span></span>
<span data-ttu-id="726a9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="726a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="726a9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="726a9-110">Permission type</span></span>|<span data-ttu-id="726a9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="726a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="726a9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="726a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="726a9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="726a9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="726a9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="726a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="726a9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="726a9-115">Not supported.</span></span>|
|<span data-ttu-id="726a9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="726a9-116">Application</span></span>|<span data-ttu-id="726a9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="726a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="726a9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="726a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="726a9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="726a9-119">Request headers</span></span>
|<span data-ttu-id="726a9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="726a9-120">Header</span></span>|<span data-ttu-id="726a9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="726a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="726a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="726a9-122">Authorization</span></span>|<span data-ttu-id="726a9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="726a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="726a9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="726a9-124">Accept</span></span>|<span data-ttu-id="726a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="726a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="726a9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="726a9-126">Request body</span></span>
<span data-ttu-id="726a9-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das macOsVppAppAssignedLicense-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="726a9-127">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="726a9-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der macOsVppAppAssignedLicense erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="726a9-128">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="726a9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="726a9-129">Property</span></span>|<span data-ttu-id="726a9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="726a9-130">Type</span></span>|<span data-ttu-id="726a9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="726a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="726a9-132">id</span><span class="sxs-lookup"><span data-stu-id="726a9-132">id</span></span>|<span data-ttu-id="726a9-133">String</span><span class="sxs-lookup"><span data-stu-id="726a9-133">String</span></span>|<span data-ttu-id="726a9-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="726a9-134">Key of the entity.</span></span>|
|<span data-ttu-id="726a9-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="726a9-135">userEmailAddress</span></span>|<span data-ttu-id="726a9-136">String</span><span class="sxs-lookup"><span data-stu-id="726a9-136">String</span></span>|<span data-ttu-id="726a9-137">Die Benutzer-e-Mail-Adresse.</span><span class="sxs-lookup"><span data-stu-id="726a9-137">The user email address.</span></span>|
|<span data-ttu-id="726a9-138">userId</span><span class="sxs-lookup"><span data-stu-id="726a9-138">userId</span></span>|<span data-ttu-id="726a9-139">String</span><span class="sxs-lookup"><span data-stu-id="726a9-139">String</span></span>|<span data-ttu-id="726a9-140">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="726a9-140">The user ID.</span></span>|
|<span data-ttu-id="726a9-141">userName</span><span class="sxs-lookup"><span data-stu-id="726a9-141">userName</span></span>|<span data-ttu-id="726a9-142">String</span><span class="sxs-lookup"><span data-stu-id="726a9-142">String</span></span>|<span data-ttu-id="726a9-143">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="726a9-143">The user name.</span></span>|
|<span data-ttu-id="726a9-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="726a9-144">userPrincipalName</span></span>|<span data-ttu-id="726a9-145">String</span><span class="sxs-lookup"><span data-stu-id="726a9-145">String</span></span>|<span data-ttu-id="726a9-146">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="726a9-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="726a9-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="726a9-147">Response</span></span>
<span data-ttu-id="726a9-148">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="726a9-148">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="726a9-149">Beispiel</span><span class="sxs-lookup"><span data-stu-id="726a9-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="726a9-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="726a9-150">Request</span></span>
<span data-ttu-id="726a9-151">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="726a9-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="726a9-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="726a9-152">Response</span></span>
<span data-ttu-id="726a9-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="726a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




