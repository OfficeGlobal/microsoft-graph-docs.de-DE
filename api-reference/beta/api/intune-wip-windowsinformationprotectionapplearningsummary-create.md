---
title: windowsInformationProtectionAppLearningSummary erstellen
description: Erstellen eines neuen windowsInformationProtectionAppLearningSummary-Objekts.
ms.openlocfilehash: 671ab1efd631541871623fd1687639dd3d8d95ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065033"
---
# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="808c9-103">windowsInformationProtectionAppLearningSummary erstellen</span><span class="sxs-lookup"><span data-stu-id="808c9-103">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="808c9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="808c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="808c9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="808c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="808c9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="808c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="808c9-107">Erstellen eines neuen [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="808c9-107">Create a new [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="808c9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="808c9-108">Prerequisites</span></span>
<span data-ttu-id="808c9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="808c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="808c9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="808c9-111">Permission type</span></span>|<span data-ttu-id="808c9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="808c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="808c9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="808c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="808c9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="808c9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="808c9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="808c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="808c9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="808c9-116">Not supported.</span></span>|
|<span data-ttu-id="808c9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="808c9-117">Application</span></span>|<span data-ttu-id="808c9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="808c9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="808c9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="808c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="808c9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="808c9-120">Request headers</span></span>
|<span data-ttu-id="808c9-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="808c9-121">Header</span></span>|<span data-ttu-id="808c9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="808c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="808c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="808c9-123">Authorization</span></span>|<span data-ttu-id="808c9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="808c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="808c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="808c9-125">Accept</span></span>|<span data-ttu-id="808c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="808c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="808c9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="808c9-127">Request body</span></span>
<span data-ttu-id="808c9-128">Geben Sie im Anforderungstext eine JSON-Darstellung des windowsInformationProtectionAppLearningSummary-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="808c9-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLearningSummary object.</span></span>

<span data-ttu-id="808c9-129">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der windowsInformationProtectionAppLearningSummary erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="808c9-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLearningSummary.</span></span>

|<span data-ttu-id="808c9-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="808c9-130">Property</span></span>|<span data-ttu-id="808c9-131">Typ</span><span class="sxs-lookup"><span data-stu-id="808c9-131">Type</span></span>|<span data-ttu-id="808c9-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="808c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="808c9-133">id</span><span class="sxs-lookup"><span data-stu-id="808c9-133">id</span></span>|<span data-ttu-id="808c9-134">String</span><span class="sxs-lookup"><span data-stu-id="808c9-134">String</span></span>|<span data-ttu-id="808c9-135">Eindeutiger Bezeichner für die WindowsInformationProtectionAppLearningSummary.</span><span class="sxs-lookup"><span data-stu-id="808c9-135">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="808c9-136">applicationName</span><span class="sxs-lookup"><span data-stu-id="808c9-136">applicationName</span></span>|<span data-ttu-id="808c9-137">String</span><span class="sxs-lookup"><span data-stu-id="808c9-137">String</span></span>|<span data-ttu-id="808c9-138">Name der Anwendung</span><span class="sxs-lookup"><span data-stu-id="808c9-138">Application Name</span></span>|
|<span data-ttu-id="808c9-139">applicationType</span><span class="sxs-lookup"><span data-stu-id="808c9-139">applicationType</span></span>|[<span data-ttu-id="808c9-140">applicationType</span><span class="sxs-lookup"><span data-stu-id="808c9-140">applicationType</span></span>](../resources/intune-wip-applicationtype.md)|<span data-ttu-id="808c9-141">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="808c9-141">Application Type.</span></span> <span data-ttu-id="808c9-142">Mögliche Werte sind: `universal` und `desktop`.</span><span class="sxs-lookup"><span data-stu-id="808c9-142">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="808c9-143">deviceCount</span><span class="sxs-lookup"><span data-stu-id="808c9-143">deviceCount</span></span>|<span data-ttu-id="808c9-144">Int32</span><span class="sxs-lookup"><span data-stu-id="808c9-144">Int32</span></span>|<span data-ttu-id="808c9-145">Geräteanzahl</span><span class="sxs-lookup"><span data-stu-id="808c9-145">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="808c9-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="808c9-146">Response</span></span>
<span data-ttu-id="808c9-147">Wenn erfolgreich, gibt diese Methode den `201 Created`-Antwortcode und das [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="808c9-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="808c9-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="808c9-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="808c9-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="808c9-149">Request</span></span>
<span data-ttu-id="808c9-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="808c9-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="808c9-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="808c9-151">Response</span></span>
<span data-ttu-id="808c9-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="808c9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```





