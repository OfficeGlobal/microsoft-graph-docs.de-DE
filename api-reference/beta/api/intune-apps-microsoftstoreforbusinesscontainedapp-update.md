---
title: MicrosoftStoreForBusinessContainedApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines MicrosoftStoreForBusinessContainedApp-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a1154555af19db7d56778d454cdc07ce647f324
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417196"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="08e3b-103">MicrosoftStoreForBusinessContainedApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="08e3b-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="08e3b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="08e3b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="08e3b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08e3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="08e3b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="08e3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08e3b-107">Aktualisieren Sie die Eigenschaften eines [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="08e3b-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08e3b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="08e3b-108">Prerequisites</span></span>
<span data-ttu-id="08e3b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="08e3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="08e3b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08e3b-111">Permission type</span></span>|<span data-ttu-id="08e3b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08e3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08e3b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08e3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08e3b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08e3b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="08e3b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08e3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08e3b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08e3b-116">Not supported.</span></span>|
|<span data-ttu-id="08e3b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08e3b-117">Application</span></span>|<span data-ttu-id="08e3b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08e3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08e3b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08e3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="08e3b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="08e3b-120">Request headers</span></span>
|<span data-ttu-id="08e3b-121">Header</span><span class="sxs-lookup"><span data-stu-id="08e3b-121">Header</span></span>|<span data-ttu-id="08e3b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="08e3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08e3b-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="08e3b-123">Authorization</span></span>|<span data-ttu-id="08e3b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="08e3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08e3b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="08e3b-125">Accept</span></span>|<span data-ttu-id="08e3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08e3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08e3b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="08e3b-127">Request body</span></span>
<span data-ttu-id="08e3b-128">Geben Sie im Textkörper Anforderung für das Objekt [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="08e3b-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="08e3b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="08e3b-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="08e3b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08e3b-130">Property</span></span>|<span data-ttu-id="08e3b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="08e3b-131">Type</span></span>|<span data-ttu-id="08e3b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08e3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08e3b-133">id</span><span class="sxs-lookup"><span data-stu-id="08e3b-133">id</span></span>|<span data-ttu-id="08e3b-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08e3b-134">String</span></span>|<span data-ttu-id="08e3b-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="08e3b-135">Key of the entity.</span></span> <span data-ttu-id="08e3b-136">Geerbt von [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="08e3b-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="08e3b-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="08e3b-137">appUserModelId</span></span>|<span data-ttu-id="08e3b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08e3b-138">String</span></span>|<span data-ttu-id="08e3b-139">Die app Benutzer Modell-ID der app enthaltenen von einer MicrosoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="08e3b-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="08e3b-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="08e3b-140">Response</span></span>
<span data-ttu-id="08e3b-141">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [MicrosoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="08e3b-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08e3b-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="08e3b-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="08e3b-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="08e3b-143">Request</span></span>
<span data-ttu-id="08e3b-144">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="08e3b-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="08e3b-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="08e3b-145">Response</span></span>
<span data-ttu-id="08e3b-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="08e3b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




