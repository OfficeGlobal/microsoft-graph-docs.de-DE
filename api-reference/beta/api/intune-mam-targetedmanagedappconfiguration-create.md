---
title: targetedManagedAppConfiguration erstellen
description: Erstellen eines neuen targetedManagedAppConfiguration-Objekts.
author: tfitzmac
ms.openlocfilehash: df5fee37bf26b34367efa9c7f6511de12125f7e2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341349"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="51714-103">targetedManagedAppConfiguration erstellen</span><span class="sxs-lookup"><span data-stu-id="51714-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="51714-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51714-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51714-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51714-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51714-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="51714-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51714-107">Erstellen eines neuen [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="51714-107">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51714-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="51714-108">Prerequisites</span></span>
<span data-ttu-id="51714-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51714-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51714-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51714-111">Permission type</span></span>|<span data-ttu-id="51714-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51714-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51714-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51714-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51714-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51714-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51714-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51714-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51714-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51714-116">Not supported.</span></span>|
|<span data-ttu-id="51714-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51714-117">Application</span></span>|<span data-ttu-id="51714-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="51714-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51714-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51714-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="51714-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51714-120">Request headers</span></span>
|<span data-ttu-id="51714-121">Header</span><span class="sxs-lookup"><span data-stu-id="51714-121">Header</span></span>|<span data-ttu-id="51714-122">Wert</span><span class="sxs-lookup"><span data-stu-id="51714-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51714-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="51714-123">Authorization</span></span>|<span data-ttu-id="51714-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="51714-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51714-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51714-125">Accept</span></span>|<span data-ttu-id="51714-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51714-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51714-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51714-127">Request body</span></span>
<span data-ttu-id="51714-128">Geben Sie im Anforderungstext eine JSON-Darstellung des targetedManagedAppConfiguration-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="51714-128">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="51714-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs targetedManagedAppConfiguration erstellen.</span><span class="sxs-lookup"><span data-stu-id="51714-129">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="51714-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="51714-130">Property</span></span>|<span data-ttu-id="51714-131">Typ</span><span class="sxs-lookup"><span data-stu-id="51714-131">Type</span></span>|<span data-ttu-id="51714-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51714-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51714-133">displayName</span><span class="sxs-lookup"><span data-stu-id="51714-133">displayName</span></span>|<span data-ttu-id="51714-134">String</span><span class="sxs-lookup"><span data-stu-id="51714-134">String</span></span>|<span data-ttu-id="51714-135">Anzeigename der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="51714-135">Policy display name.</span></span> <span data-ttu-id="51714-136">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="51714-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="51714-137">description</span><span class="sxs-lookup"><span data-stu-id="51714-137">description</span></span>|<span data-ttu-id="51714-138">String</span><span class="sxs-lookup"><span data-stu-id="51714-138">String</span></span>|<span data-ttu-id="51714-139">Beschreibung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="51714-139">The policy's description.</span></span> <span data-ttu-id="51714-140">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="51714-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="51714-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51714-141">createdDateTime</span></span>|<span data-ttu-id="51714-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51714-142">DateTimeOffset</span></span>|<span data-ttu-id="51714-143">Datum und Uhrzeit der Erstellung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="51714-143">The date and time the policy was created.</span></span> <span data-ttu-id="51714-144">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="51714-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="51714-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51714-145">lastModifiedDateTime</span></span>|<span data-ttu-id="51714-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51714-146">DateTimeOffset</span></span>|<span data-ttu-id="51714-147">Datum und Uhrzeit der letzten Änderung der Richtlinie</span><span class="sxs-lookup"><span data-stu-id="51714-147">Last time the policy was modified.</span></span> <span data-ttu-id="51714-148">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="51714-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="51714-149">id</span><span class="sxs-lookup"><span data-stu-id="51714-149">id</span></span>|<span data-ttu-id="51714-150">String</span><span class="sxs-lookup"><span data-stu-id="51714-150">String</span></span>|<span data-ttu-id="51714-151">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="51714-151">Key of the entity.</span></span> <span data-ttu-id="51714-152">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="51714-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="51714-153">Version</span><span class="sxs-lookup"><span data-stu-id="51714-153">version</span></span>|<span data-ttu-id="51714-154">String</span><span class="sxs-lookup"><span data-stu-id="51714-154">String</span></span>|<span data-ttu-id="51714-155">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="51714-155">Version of the entity.</span></span> <span data-ttu-id="51714-156">Geerbt von [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).</span><span class="sxs-lookup"><span data-stu-id="51714-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="51714-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="51714-157">customSettings</span></span>|<span data-ttu-id="51714-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="51714-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="51714-159">Eine Gruppe von Paaren aus Schlüsselzeichenfolge und Wertzeichenfolge, die an Apps für Benutzer im Bereich der Konfiguration gesendet werden sollen, und zwar ohne Veränderungen durch den Dienst. Geerbt von [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51714-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="51714-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="51714-160">deployedAppCount</span></span>|<span data-ttu-id="51714-161">Int32</span><span class="sxs-lookup"><span data-stu-id="51714-161">Int32</span></span>|<span data-ttu-id="51714-162">Anzahl der Apps, für die die aktuelle Richtlinie bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="51714-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="51714-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="51714-163">isAssigned</span></span>|<span data-ttu-id="51714-164">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="51714-164">Boolean</span></span>|<span data-ttu-id="51714-165">Gibt an, ob die Richtlinie für eine oder mehrere Einschlussgruppen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="51714-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="51714-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="51714-166">Response</span></span>
<span data-ttu-id="51714-167">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51714-167">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51714-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51714-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="51714-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="51714-169">Request</span></span>
<span data-ttu-id="51714-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="51714-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="51714-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="51714-171">Response</span></span>
<span data-ttu-id="51714-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="51714-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





