---
title: IosVppAppAssignedUserLicense aktualisieren
description: Aktualisieren Sie die Eigenschaften eines IosVppAppAssignedUserLicense-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ea6aa8383c363744278929a1f1cd84eb1605e055
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870080"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="f8e76-103">IosVppAppAssignedUserLicense aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f8e76-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="f8e76-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f8e76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8e76-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8e76-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8e76-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f8e76-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8e76-107">Aktualisieren Sie die Eigenschaften eines [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f8e76-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8e76-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f8e76-108">Prerequisites</span></span>
<span data-ttu-id="f8e76-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8e76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8e76-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8e76-111">Permission type</span></span>|<span data-ttu-id="f8e76-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8e76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8e76-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8e76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8e76-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8e76-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f8e76-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8e76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8e76-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8e76-116">Not supported.</span></span>|
|<span data-ttu-id="f8e76-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8e76-117">Application</span></span>|<span data-ttu-id="f8e76-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8e76-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8e76-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8e76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="f8e76-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8e76-120">Request headers</span></span>
|<span data-ttu-id="f8e76-121">Header</span><span class="sxs-lookup"><span data-stu-id="f8e76-121">Header</span></span>|<span data-ttu-id="f8e76-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f8e76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8e76-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8e76-123">Authorization</span></span>|<span data-ttu-id="f8e76-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f8e76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8e76-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f8e76-125">Accept</span></span>|<span data-ttu-id="f8e76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8e76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8e76-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8e76-127">Request body</span></span>
<span data-ttu-id="f8e76-128">Geben Sie im Textkörper Anforderung für das Objekt [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f8e76-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="f8e76-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="f8e76-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="f8e76-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f8e76-130">Property</span></span>|<span data-ttu-id="f8e76-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f8e76-131">Type</span></span>|<span data-ttu-id="f8e76-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8e76-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8e76-133">id</span><span class="sxs-lookup"><span data-stu-id="f8e76-133">id</span></span>|<span data-ttu-id="f8e76-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8e76-134">String</span></span>|<span data-ttu-id="f8e76-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="f8e76-135">Key of the entity.</span></span> <span data-ttu-id="f8e76-136">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8e76-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f8e76-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f8e76-137">userEmailAddress</span></span>|<span data-ttu-id="f8e76-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8e76-138">String</span></span>|<span data-ttu-id="f8e76-139">Die e-Mail-Adresse des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f8e76-139">The user email address.</span></span> <span data-ttu-id="f8e76-140">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8e76-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f8e76-141">userId</span><span class="sxs-lookup"><span data-stu-id="f8e76-141">userId</span></span>|<span data-ttu-id="f8e76-142">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8e76-142">String</span></span>|<span data-ttu-id="f8e76-143">Die Benutzer-ID.</span><span class="sxs-lookup"><span data-stu-id="f8e76-143">The user ID.</span></span> <span data-ttu-id="f8e76-144">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8e76-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f8e76-145">userName</span><span class="sxs-lookup"><span data-stu-id="f8e76-145">userName</span></span>|<span data-ttu-id="f8e76-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8e76-146">String</span></span>|<span data-ttu-id="f8e76-147">Der Benutzername.</span><span class="sxs-lookup"><span data-stu-id="f8e76-147">The user name.</span></span> <span data-ttu-id="f8e76-148">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8e76-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="f8e76-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8e76-149">userPrincipalName</span></span>|<span data-ttu-id="f8e76-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f8e76-150">String</span></span>|<span data-ttu-id="f8e76-151">Der Benutzerprinzipalname.</span><span class="sxs-lookup"><span data-stu-id="f8e76-151">The user principal name.</span></span> <span data-ttu-id="f8e76-152">Geerbt von [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="f8e76-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f8e76-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8e76-153">Response</span></span>
<span data-ttu-id="f8e76-154">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [IosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f8e76-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8e76-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8e76-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8e76-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8e76-156">Request</span></span>
<span data-ttu-id="f8e76-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8e76-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 171

{
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="f8e76-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8e76-158">Response</span></span>
<span data-ttu-id="f8e76-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8e76-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





