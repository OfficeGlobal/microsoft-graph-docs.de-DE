---
title: MacOsVppAppAssignedLicense aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MacOsVppAppAssignedLicense-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0e3a8a2c54035a29225be547c9971d70fb70f92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431552"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="97cf7-103">MacOsVppAppAssignedLicense aktualisieren</span><span class="sxs-lookup"><span data-stu-id="97cf7-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="97cf7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="97cf7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97cf7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97cf7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97cf7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97cf7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97cf7-107">Aktualisieren Sie die Eigenschaften eines [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="97cf7-107">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97cf7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="97cf7-108">Prerequisites</span></span>
<span data-ttu-id="97cf7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="97cf7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="97cf7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97cf7-111">Permission type</span></span>|<span data-ttu-id="97cf7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97cf7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97cf7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97cf7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97cf7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97cf7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="97cf7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97cf7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97cf7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97cf7-116">Not supported.</span></span>|
|<span data-ttu-id="97cf7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97cf7-117">Application</span></span>|<span data-ttu-id="97cf7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97cf7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97cf7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97cf7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="97cf7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97cf7-120">Request headers</span></span>
|<span data-ttu-id="97cf7-121">Header</span><span class="sxs-lookup"><span data-stu-id="97cf7-121">Header</span></span>|<span data-ttu-id="97cf7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="97cf7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97cf7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="97cf7-123">Authorization</span></span>|<span data-ttu-id="97cf7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="97cf7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97cf7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="97cf7-125">Accept</span></span>|<span data-ttu-id="97cf7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97cf7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97cf7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97cf7-127">Request body</span></span>
<span data-ttu-id="97cf7-128">Geben Sie im Textkörper Anforderung für das Objekt [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="97cf7-128">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="97cf7-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="97cf7-129">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="97cf7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97cf7-130">Property</span></span>|<span data-ttu-id="97cf7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="97cf7-131">Type</span></span>|<span data-ttu-id="97cf7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97cf7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97cf7-133">id</span><span class="sxs-lookup"><span data-stu-id="97cf7-133">id</span></span>|<span data-ttu-id="97cf7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97cf7-134">String</span></span>|<span data-ttu-id="97cf7-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="97cf7-135">Key of the entity.</span></span>|
|<span data-ttu-id="97cf7-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="97cf7-136">userEmailAddress</span></span>|<span data-ttu-id="97cf7-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97cf7-137">String</span></span>|<span data-ttu-id="97cf7-138">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="97cf7-138">The user email address.</span></span>|
|<span data-ttu-id="97cf7-139">userId</span><span class="sxs-lookup"><span data-stu-id="97cf7-139">userId</span></span>|<span data-ttu-id="97cf7-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97cf7-140">String</span></span>|<span data-ttu-id="97cf7-141">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="97cf7-141">The user ID.</span></span>|
|<span data-ttu-id="97cf7-142">userName</span><span class="sxs-lookup"><span data-stu-id="97cf7-142">userName</span></span>|<span data-ttu-id="97cf7-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97cf7-143">String</span></span>|<span data-ttu-id="97cf7-144">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="97cf7-144">The user name.</span></span>|
|<span data-ttu-id="97cf7-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="97cf7-145">userPrincipalName</span></span>|<span data-ttu-id="97cf7-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97cf7-146">String</span></span>|<span data-ttu-id="97cf7-147">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="97cf7-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="97cf7-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="97cf7-148">Response</span></span>
<span data-ttu-id="97cf7-149">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MacOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="97cf7-149">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97cf7-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97cf7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="97cf7-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97cf7-151">Request</span></span>
<span data-ttu-id="97cf7-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97cf7-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="97cf7-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="97cf7-153">Response</span></span>
<span data-ttu-id="97cf7-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97cf7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




