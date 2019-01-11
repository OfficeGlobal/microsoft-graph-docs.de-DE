---
title: Erstellen von windowsUniversalAppXContainedApp
description: Erstellen eines neuen WindowsUniversalAppXContainedApp-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 283852a1539fd16bb6c19f9db0d1770d9eb7e466
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863826"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="c69e0-103">Erstellen von windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="c69e0-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="c69e0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c69e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c69e0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c69e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c69e0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c69e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c69e0-107">Erstellen eines neuen [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c69e0-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c69e0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c69e0-108">Prerequisites</span></span>
<span data-ttu-id="c69e0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c69e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c69e0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c69e0-111">Permission type</span></span>|<span data-ttu-id="c69e0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c69e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c69e0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c69e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c69e0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c69e0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c69e0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c69e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c69e0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c69e0-116">Not supported.</span></span>|
|<span data-ttu-id="c69e0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c69e0-117">Application</span></span>|<span data-ttu-id="c69e0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c69e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c69e0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c69e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="c69e0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c69e0-120">Request headers</span></span>
|<span data-ttu-id="c69e0-121">Header</span><span class="sxs-lookup"><span data-stu-id="c69e0-121">Header</span></span>|<span data-ttu-id="c69e0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c69e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c69e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c69e0-123">Authorization</span></span>|<span data-ttu-id="c69e0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c69e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c69e0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c69e0-125">Accept</span></span>|<span data-ttu-id="c69e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c69e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c69e0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c69e0-127">Request body</span></span>
<span data-ttu-id="c69e0-128">Geben Sie im Textkörper Anforderung für das Objekt WindowsUniversalAppXContainedApp eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c69e0-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="c69e0-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die WindowsUniversalAppXContainedApp erstellen.</span><span class="sxs-lookup"><span data-stu-id="c69e0-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="c69e0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c69e0-130">Property</span></span>|<span data-ttu-id="c69e0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c69e0-131">Type</span></span>|<span data-ttu-id="c69e0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c69e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c69e0-133">id</span><span class="sxs-lookup"><span data-stu-id="c69e0-133">id</span></span>|<span data-ttu-id="c69e0-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c69e0-134">String</span></span>|<span data-ttu-id="c69e0-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c69e0-135">Key of the entity.</span></span> <span data-ttu-id="c69e0-136">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c69e0-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="c69e0-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="c69e0-137">appUserModelId</span></span>|<span data-ttu-id="c69e0-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c69e0-138">String</span></span>|<span data-ttu-id="c69e0-139">Die app Benutzer Modell-ID der app enthaltenen einer WindowsUniversalAppX-App.</span><span class="sxs-lookup"><span data-stu-id="c69e0-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="c69e0-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="c69e0-140">Response</span></span>
<span data-ttu-id="c69e0-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c69e0-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c69e0-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c69e0-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="c69e0-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c69e0-143">Request</span></span>
<span data-ttu-id="c69e0-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c69e0-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="c69e0-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="c69e0-145">Response</span></span>
<span data-ttu-id="c69e0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c69e0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```





