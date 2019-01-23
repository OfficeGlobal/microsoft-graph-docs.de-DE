---
title: Erstellen von macOsVppAppAssignedLicense
description: Erstellen eines neuen MacOsVppAppAssignedLicense-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07c0bafef2eb86128c8d9bc8cfb071b45bc1e913
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430078"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="ca159-103">Erstellen von macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="ca159-103">Create macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="ca159-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ca159-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca159-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca159-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca159-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ca159-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca159-107">Erstellen eines neuen [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ca159-107">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca159-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ca159-108">Prerequisites</span></span>
<span data-ttu-id="ca159-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca159-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ca159-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ca159-111">Permission type</span></span>|<span data-ttu-id="ca159-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ca159-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca159-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ca159-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca159-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca159-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ca159-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ca159-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca159-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca159-116">Not supported.</span></span>|
|<span data-ttu-id="ca159-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ca159-117">Application</span></span>|<span data-ttu-id="ca159-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca159-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca159-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca159-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="ca159-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ca159-120">Request headers</span></span>
|<span data-ttu-id="ca159-121">Header</span><span class="sxs-lookup"><span data-stu-id="ca159-121">Header</span></span>|<span data-ttu-id="ca159-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ca159-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca159-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ca159-123">Authorization</span></span>|<span data-ttu-id="ca159-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ca159-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca159-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ca159-125">Accept</span></span>|<span data-ttu-id="ca159-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca159-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca159-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ca159-127">Request body</span></span>
<span data-ttu-id="ca159-128">Geben Sie im Textkörper Anforderung für das Objekt MacOsVppAppAssignedLicense eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="ca159-128">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="ca159-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die MacOsVppAppAssignedLicense erstellen.</span><span class="sxs-lookup"><span data-stu-id="ca159-129">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="ca159-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ca159-130">Property</span></span>|<span data-ttu-id="ca159-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ca159-131">Type</span></span>|<span data-ttu-id="ca159-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ca159-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca159-133">id</span><span class="sxs-lookup"><span data-stu-id="ca159-133">id</span></span>|<span data-ttu-id="ca159-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca159-134">String</span></span>|<span data-ttu-id="ca159-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ca159-135">Key of the entity.</span></span>|
|<span data-ttu-id="ca159-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ca159-136">userEmailAddress</span></span>|<span data-ttu-id="ca159-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca159-137">String</span></span>|<span data-ttu-id="ca159-138">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="ca159-138">The user email address.</span></span>|
|<span data-ttu-id="ca159-139">userId</span><span class="sxs-lookup"><span data-stu-id="ca159-139">userId</span></span>|<span data-ttu-id="ca159-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca159-140">String</span></span>|<span data-ttu-id="ca159-141">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="ca159-141">The user ID.</span></span>|
|<span data-ttu-id="ca159-142">userName</span><span class="sxs-lookup"><span data-stu-id="ca159-142">userName</span></span>|<span data-ttu-id="ca159-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca159-143">String</span></span>|<span data-ttu-id="ca159-144">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="ca159-144">The user name.</span></span>|
|<span data-ttu-id="ca159-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ca159-145">userPrincipalName</span></span>|<span data-ttu-id="ca159-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ca159-146">String</span></span>|<span data-ttu-id="ca159-147">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="ca159-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="ca159-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca159-148">Response</span></span>
<span data-ttu-id="ca159-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="ca159-149">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca159-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ca159-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca159-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca159-151">Request</span></span>
<span data-ttu-id="ca159-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ca159-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca159-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca159-153">Response</span></span>
<span data-ttu-id="ca159-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca159-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




