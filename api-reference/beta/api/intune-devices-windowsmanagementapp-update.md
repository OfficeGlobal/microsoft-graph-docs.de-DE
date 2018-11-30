---
title: WindowsManagementApp aktualisieren
description: Aktualisieren Sie die Eigenschaften eines WindowsManagementApp-Objekts.
ms.openlocfilehash: 88a0511a06c94a4c5298fc53fa19b512f723177d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059788"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="5efb3-103">WindowsManagementApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="5efb3-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="5efb3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5efb3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5efb3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5efb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5efb3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5efb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5efb3-107">Aktualisieren Sie die Eigenschaften eines [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5efb3-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5efb3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5efb3-108">Prerequisites</span></span>
<span data-ttu-id="5efb3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5efb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5efb3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5efb3-111">Permission type</span></span>|<span data-ttu-id="5efb3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5efb3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5efb3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5efb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5efb3-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5efb3-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5efb3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5efb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5efb3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5efb3-116">Not supported.</span></span>|
|<span data-ttu-id="5efb3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5efb3-117">Application</span></span>|<span data-ttu-id="5efb3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5efb3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5efb3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5efb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="5efb3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5efb3-120">Request headers</span></span>
|<span data-ttu-id="5efb3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5efb3-121">Header</span></span>|<span data-ttu-id="5efb3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="5efb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5efb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5efb3-123">Authorization</span></span>|<span data-ttu-id="5efb3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5efb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5efb3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5efb3-125">Accept</span></span>|<span data-ttu-id="5efb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5efb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5efb3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5efb3-127">Request body</span></span>
<span data-ttu-id="5efb3-128">Geben Sie im Textkörper Anforderung für das Objekt [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="5efb3-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="5efb3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="5efb3-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="5efb3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5efb3-130">Property</span></span>|<span data-ttu-id="5efb3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="5efb3-131">Type</span></span>|<span data-ttu-id="5efb3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5efb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5efb3-133">id</span><span class="sxs-lookup"><span data-stu-id="5efb3-133">id</span></span>|<span data-ttu-id="5efb3-134">String</span><span class="sxs-lookup"><span data-stu-id="5efb3-134">String</span></span>|<span data-ttu-id="5efb3-135">Eindeutiger Bezeichner für die Windows Management-app</span><span class="sxs-lookup"><span data-stu-id="5efb3-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="5efb3-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="5efb3-136">availableVersion</span></span>|<span data-ttu-id="5efb3-137">String</span><span class="sxs-lookup"><span data-stu-id="5efb3-137">String</span></span>|<span data-ttu-id="5efb3-138">Windows Management app verfügbare Version.</span><span class="sxs-lookup"><span data-stu-id="5efb3-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="5efb3-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="5efb3-139">Response</span></span>
<span data-ttu-id="5efb3-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5efb3-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5efb3-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5efb3-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="5efb3-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5efb3-142">Request</span></span>
<span data-ttu-id="5efb3-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5efb3-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 53

{
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="5efb3-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="5efb3-144">Response</span></span>
<span data-ttu-id="5efb3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5efb3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```





