---
title: WindowsUniversalAppXContainedApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsUniversalAppXContainedApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b396d7d1c2995f9e65db63622ad421a481cfe9de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405611"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="0506c-103">WindowsUniversalAppXContainedApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0506c-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="0506c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0506c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0506c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0506c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0506c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0506c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0506c-107">Aktualisieren Sie die Eigenschaften eines [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0506c-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0506c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0506c-108">Prerequisites</span></span>
<span data-ttu-id="0506c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0506c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0506c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0506c-111">Permission type</span></span>|<span data-ttu-id="0506c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0506c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0506c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0506c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0506c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0506c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0506c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0506c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0506c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0506c-116">Not supported.</span></span>|
|<span data-ttu-id="0506c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0506c-117">Application</span></span>|<span data-ttu-id="0506c-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0506c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0506c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0506c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0506c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0506c-120">Request headers</span></span>
|<span data-ttu-id="0506c-121">Header</span><span class="sxs-lookup"><span data-stu-id="0506c-121">Header</span></span>|<span data-ttu-id="0506c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0506c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0506c-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0506c-123">Authorization</span></span>|<span data-ttu-id="0506c-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0506c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0506c-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0506c-125">Accept</span></span>|<span data-ttu-id="0506c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0506c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0506c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0506c-127">Request body</span></span>
<span data-ttu-id="0506c-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0506c-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="0506c-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0506c-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="0506c-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0506c-130">Property</span></span>|<span data-ttu-id="0506c-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0506c-131">Type</span></span>|<span data-ttu-id="0506c-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0506c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0506c-133">id</span><span class="sxs-lookup"><span data-stu-id="0506c-133">id</span></span>|<span data-ttu-id="0506c-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0506c-134">String</span></span>|<span data-ttu-id="0506c-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0506c-135">Key of the entity.</span></span> <span data-ttu-id="0506c-136">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="0506c-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="0506c-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="0506c-137">appUserModelId</span></span>|<span data-ttu-id="0506c-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0506c-138">String</span></span>|<span data-ttu-id="0506c-139">Die app Benutzer Modell-ID der app enthaltenen einer WindowsUniversalAppX-App.</span><span class="sxs-lookup"><span data-stu-id="0506c-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="0506c-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0506c-140">Response</span></span>
<span data-ttu-id="0506c-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0506c-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0506c-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0506c-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="0506c-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0506c-143">Request</span></span>
<span data-ttu-id="0506c-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0506c-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="0506c-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0506c-145">Response</span></span>
<span data-ttu-id="0506c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0506c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




