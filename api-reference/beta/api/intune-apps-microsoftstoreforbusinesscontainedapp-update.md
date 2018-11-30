---
title: MicrosoftStoreForBusinessContainedApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MicrosoftStoreForBusinessContainedApp-Objekts.
ms.openlocfilehash: b5a946a79b5040778cce24deaee3326f93380e76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065796"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="0460e-103">MicrosoftStoreForBusinessContainedApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0460e-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="0460e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0460e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0460e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0460e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0460e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0460e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0460e-107">Aktualisieren Sie die Eigenschaften eines [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0460e-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0460e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0460e-108">Prerequisites</span></span>
<span data-ttu-id="0460e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0460e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0460e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0460e-111">Permission type</span></span>|<span data-ttu-id="0460e-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0460e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0460e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0460e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0460e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0460e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0460e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0460e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0460e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0460e-116">Not supported.</span></span>|
|<span data-ttu-id="0460e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0460e-117">Application</span></span>|<span data-ttu-id="0460e-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0460e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0460e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0460e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0460e-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0460e-120">Request headers</span></span>
|<span data-ttu-id="0460e-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0460e-121">Header</span></span>|<span data-ttu-id="0460e-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0460e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0460e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0460e-123">Authorization</span></span>|<span data-ttu-id="0460e-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0460e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0460e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0460e-125">Accept</span></span>|<span data-ttu-id="0460e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0460e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0460e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0460e-127">Request body</span></span>
<span data-ttu-id="0460e-128">Geben Sie im Textkörper Anforderung für das Objekt [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="0460e-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="0460e-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="0460e-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="0460e-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0460e-130">Property</span></span>|<span data-ttu-id="0460e-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0460e-131">Type</span></span>|<span data-ttu-id="0460e-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0460e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0460e-133">id</span><span class="sxs-lookup"><span data-stu-id="0460e-133">id</span></span>|<span data-ttu-id="0460e-134">String</span><span class="sxs-lookup"><span data-stu-id="0460e-134">String</span></span>|<span data-ttu-id="0460e-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0460e-135">Key of the entity.</span></span> <span data-ttu-id="0460e-136">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="0460e-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="0460e-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="0460e-137">appUserModelId</span></span>|<span data-ttu-id="0460e-138">String</span><span class="sxs-lookup"><span data-stu-id="0460e-138">String</span></span>|<span data-ttu-id="0460e-139">Die app Benutzer Modell-ID der app enthaltenen von einer MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="0460e-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="0460e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0460e-140">Response</span></span>
<span data-ttu-id="0460e-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0460e-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0460e-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0460e-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="0460e-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0460e-143">Request</span></span>
<span data-ttu-id="0460e-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0460e-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 51

{
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="0460e-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0460e-145">Response</span></span>
<span data-ttu-id="0460e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0460e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```





