---
title: WindowsUniversalAppXContainedApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsUniversalAppXContainedApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 642921c66bfbc996c5c3b0f3f16cf812c75a5618
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882341"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="5ae45-103">WindowsUniversalAppXContainedApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5ae45-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="5ae45-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5ae45-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ae45-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5ae45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ae45-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5ae45-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ae45-107">Aktualisieren Sie die Eigenschaften eines [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5ae45-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ae45-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5ae45-108">Prerequisites</span></span>
<span data-ttu-id="5ae45-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ae45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ae45-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5ae45-111">Permission type</span></span>|<span data-ttu-id="5ae45-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5ae45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ae45-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5ae45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ae45-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae45-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5ae45-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5ae45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ae45-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ae45-116">Not supported.</span></span>|
|<span data-ttu-id="5ae45-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5ae45-117">Application</span></span>|<span data-ttu-id="5ae45-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5ae45-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ae45-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ae45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="5ae45-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5ae45-120">Request headers</span></span>
|<span data-ttu-id="5ae45-121">Header</span><span class="sxs-lookup"><span data-stu-id="5ae45-121">Header</span></span>|<span data-ttu-id="5ae45-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5ae45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ae45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ae45-123">Authorization</span></span>|<span data-ttu-id="5ae45-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5ae45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ae45-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5ae45-125">Accept</span></span>|<span data-ttu-id="5ae45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ae45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ae45-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ae45-127">Request body</span></span>
<span data-ttu-id="5ae45-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5ae45-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="5ae45-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="5ae45-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="5ae45-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5ae45-130">Property</span></span>|<span data-ttu-id="5ae45-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5ae45-131">Type</span></span>|<span data-ttu-id="5ae45-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5ae45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ae45-133">id</span><span class="sxs-lookup"><span data-stu-id="5ae45-133">id</span></span>|<span data-ttu-id="5ae45-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5ae45-134">String</span></span>|<span data-ttu-id="5ae45-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5ae45-135">Key of the entity.</span></span> <span data-ttu-id="5ae45-136">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ae45-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="5ae45-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="5ae45-137">appUserModelId</span></span>|<span data-ttu-id="5ae45-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5ae45-138">String</span></span>|<span data-ttu-id="5ae45-139">Die app Benutzer Modell-ID der app enthaltenen einer WindowsUniversalAppX-App.</span><span class="sxs-lookup"><span data-stu-id="5ae45-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="5ae45-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ae45-140">Response</span></span>
<span data-ttu-id="5ae45-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5ae45-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ae45-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ae45-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ae45-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ae45-143">Request</span></span>
<span data-ttu-id="5ae45-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5ae45-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 51

{
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="5ae45-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ae45-145">Response</span></span>
<span data-ttu-id="5ae45-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5ae45-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```





