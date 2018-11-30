---
title: targetedManagedAppConfiguration erstellen
description: Erstellen eines neuen targetedManagedAppConfiguration-Objekts.
ms.openlocfilehash: 0bf32ede52b1fc09ff8729248df75de0ca14a94d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016832"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="94b7f-103">targetedManagedAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="94b7f-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="94b7f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="94b7f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94b7f-105">Erstellen eines neuen [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="94b7f-105">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94b7f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="94b7f-106">Prerequisites</span></span>
<span data-ttu-id="94b7f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94b7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94b7f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="94b7f-109">Permission type</span></span>|<span data-ttu-id="94b7f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="94b7f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94b7f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="94b7f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94b7f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94b7f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="94b7f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="94b7f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94b7f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94b7f-114">Not supported.</span></span>|
|<span data-ttu-id="94b7f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="94b7f-115">Application</span></span>|<span data-ttu-id="94b7f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="94b7f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94b7f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="94b7f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="94b7f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="94b7f-118">Request headers</span></span>
|<span data-ttu-id="94b7f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="94b7f-119">Header</span></span>|<span data-ttu-id="94b7f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="94b7f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94b7f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="94b7f-121">Authorization</span></span>|<span data-ttu-id="94b7f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="94b7f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94b7f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="94b7f-123">Accept</span></span>|<span data-ttu-id="94b7f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="94b7f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94b7f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="94b7f-125">Request body</span></span>
<span data-ttu-id="94b7f-126">Geben Sie im Anforderungstext eine JSON-Darstellung des targetedManagedAppConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="94b7f-126">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="94b7f-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs targetedManagedAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="94b7f-127">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="94b7f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="94b7f-128">Property</span></span>|<span data-ttu-id="94b7f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="94b7f-129">Type</span></span>|<span data-ttu-id="94b7f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="94b7f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94b7f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="94b7f-131">displayName</span></span>|<span data-ttu-id="94b7f-132">String</span><span class="sxs-lookup"><span data-stu-id="94b7f-132">String</span></span>|<span data-ttu-id="94b7f-133">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="94b7f-133">Policy display name.</span></span> <span data-ttu-id="94b7f-134">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="94b7f-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="94b7f-135">description</span><span class="sxs-lookup"><span data-stu-id="94b7f-135">description</span></span>|<span data-ttu-id="94b7f-136">String</span><span class="sxs-lookup"><span data-stu-id="94b7f-136">String</span></span>|<span data-ttu-id="94b7f-137">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="94b7f-137">The policy's description.</span></span> <span data-ttu-id="94b7f-138">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="94b7f-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="94b7f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94b7f-139">createdDateTime</span></span>|<span data-ttu-id="94b7f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94b7f-140">DateTimeOffset</span></span>|<span data-ttu-id="94b7f-141">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="94b7f-141">The date and time the policy was created.</span></span> <span data-ttu-id="94b7f-142">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="94b7f-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="94b7f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94b7f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="94b7f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94b7f-144">DateTimeOffset</span></span>|<span data-ttu-id="94b7f-145">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="94b7f-145">Last time the policy was modified.</span></span> <span data-ttu-id="94b7f-146">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="94b7f-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="94b7f-147">id</span><span class="sxs-lookup"><span data-stu-id="94b7f-147">id</span></span>|<span data-ttu-id="94b7f-148">String</span><span class="sxs-lookup"><span data-stu-id="94b7f-148">String</span></span>|<span data-ttu-id="94b7f-149">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="94b7f-149">Key of the entity.</span></span> <span data-ttu-id="94b7f-150">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="94b7f-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="94b7f-151">Version</span><span class="sxs-lookup"><span data-stu-id="94b7f-151">version</span></span>|<span data-ttu-id="94b7f-152">String</span><span class="sxs-lookup"><span data-stu-id="94b7f-152">String</span></span>|<span data-ttu-id="94b7f-153">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="94b7f-153">Version of the entity.</span></span> <span data-ttu-id="94b7f-154">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="94b7f-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="94b7f-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="94b7f-155">customSettings</span></span>|<span data-ttu-id="94b7f-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="94b7f-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="94b7f-157">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="94b7f-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="94b7f-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="94b7f-158">deployedAppCount</span></span>|<span data-ttu-id="94b7f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="94b7f-159">Int32</span></span>|<span data-ttu-id="94b7f-160">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="94b7f-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="94b7f-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="94b7f-161">isAssigned</span></span>|<span data-ttu-id="94b7f-162">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="94b7f-162">Boolean</span></span>|<span data-ttu-id="94b7f-163">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="94b7f-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="94b7f-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="94b7f-164">Response</span></span>
<span data-ttu-id="94b7f-165">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94b7f-165">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94b7f-166">Beispiel</span><span class="sxs-lookup"><span data-stu-id="94b7f-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="94b7f-167">Anforderung</span><span class="sxs-lookup"><span data-stu-id="94b7f-167">Request</span></span>
<span data-ttu-id="94b7f-168">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="94b7f-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="94b7f-169">Antwort</span><span class="sxs-lookup"><span data-stu-id="94b7f-169">Response</span></span>
<span data-ttu-id="94b7f-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="94b7f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```



