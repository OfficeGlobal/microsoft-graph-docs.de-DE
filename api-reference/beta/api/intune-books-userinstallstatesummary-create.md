---
title: Erstellen von „userInstallStateSummary“
description: Diese Methode erstellt ein neues Objekt des Typs userInstallStateSummary.
author: tfitzmac
ms.openlocfilehash: 1f90c76382379f1e448c02d5b83a415c9a97fc82
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350288"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="ebb5f-103">Erstellen von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="ebb5f-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="ebb5f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ebb5f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebb5f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ebb5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebb5f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ebb5f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebb5f-107">Diese Methode erstellt ein neues Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ebb5f-107">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ebb5f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ebb5f-108">Prerequisites</span></span>
<span data-ttu-id="ebb5f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebb5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebb5f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ebb5f-111">Permission type</span></span>|<span data-ttu-id="ebb5f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ebb5f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebb5f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ebb5f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebb5f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebb5f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ebb5f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ebb5f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebb5f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebb5f-116">Not supported.</span></span>|
|<span data-ttu-id="ebb5f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ebb5f-117">Application</span></span>|<span data-ttu-id="ebb5f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ebb5f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebb5f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebb5f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="ebb5f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ebb5f-120">Request headers</span></span>
|<span data-ttu-id="ebb5f-121">Header</span><span class="sxs-lookup"><span data-stu-id="ebb5f-121">Header</span></span>|<span data-ttu-id="ebb5f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ebb5f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebb5f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ebb5f-123">Authorization</span></span>|<span data-ttu-id="ebb5f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ebb5f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebb5f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ebb5f-125">Accept</span></span>|<span data-ttu-id="ebb5f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebb5f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebb5f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ebb5f-127">Request body</span></span>
<span data-ttu-id="ebb5f-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „userInstallStateSummary“ an.</span><span class="sxs-lookup"><span data-stu-id="ebb5f-128">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="ebb5f-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „userInstallStateSummary“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="ebb5f-129">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="ebb5f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ebb5f-130">Property</span></span>|<span data-ttu-id="ebb5f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ebb5f-131">Type</span></span>|<span data-ttu-id="ebb5f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ebb5f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebb5f-133">id</span><span class="sxs-lookup"><span data-stu-id="ebb5f-133">id</span></span>|<span data-ttu-id="ebb5f-134">String</span><span class="sxs-lookup"><span data-stu-id="ebb5f-134">String</span></span>|<span data-ttu-id="ebb5f-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ebb5f-135">Key of the entity.</span></span>|
|<span data-ttu-id="ebb5f-136">userName</span><span class="sxs-lookup"><span data-stu-id="ebb5f-136">userName</span></span>|<span data-ttu-id="ebb5f-137">String</span><span class="sxs-lookup"><span data-stu-id="ebb5f-137">String</span></span>|<span data-ttu-id="ebb5f-138">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="ebb5f-138">User name.</span></span>|
|<span data-ttu-id="ebb5f-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebb5f-139">installedDeviceCount</span></span>|<span data-ttu-id="ebb5f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ebb5f-140">Int32</span></span>|<span data-ttu-id="ebb5f-141">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="ebb5f-141">Installed Device Count.</span></span>|
|<span data-ttu-id="ebb5f-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebb5f-142">failedDeviceCount</span></span>|<span data-ttu-id="ebb5f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ebb5f-143">Int32</span></span>|<span data-ttu-id="ebb5f-144">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="ebb5f-144">Failed Device Count.</span></span>|
|<span data-ttu-id="ebb5f-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebb5f-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="ebb5f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ebb5f-146">Int32</span></span>|<span data-ttu-id="ebb5f-147">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="ebb5f-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="ebb5f-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebb5f-148">Response</span></span>
<span data-ttu-id="ebb5f-149">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ebb5f-149">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebb5f-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ebb5f-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="ebb5f-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ebb5f-151">Request</span></span>
<span data-ttu-id="ebb5f-152">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ebb5f-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="ebb5f-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="ebb5f-153">Response</span></span>
<span data-ttu-id="ebb5f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ebb5f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```





