---
title: Erstellen von „userInstallStateSummary“
description: Diese Methode erstellt ein neues Objekt des Typs userInstallStateSummary.
author: tfitzmac
ms.openlocfilehash: a1da2855896bae9d9c902ae978d3ce8c127f3bc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318417"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="73ba6-103">Erstellen von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="73ba6-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="73ba6-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73ba6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73ba6-105">Diese Methode erstellt ein neues Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="73ba6-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73ba6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="73ba6-106">Prerequisites</span></span>
<span data-ttu-id="73ba6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73ba6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73ba6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73ba6-109">Permission type</span></span>|<span data-ttu-id="73ba6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73ba6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73ba6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73ba6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="73ba6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73ba6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73ba6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73ba6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73ba6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73ba6-114">Not supported.</span></span>|
|<span data-ttu-id="73ba6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73ba6-115">Application</span></span>|<span data-ttu-id="73ba6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73ba6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73ba6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73ba6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="73ba6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73ba6-118">Request headers</span></span>
|<span data-ttu-id="73ba6-119">Header</span><span class="sxs-lookup"><span data-stu-id="73ba6-119">Header</span></span>|<span data-ttu-id="73ba6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="73ba6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73ba6-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="73ba6-121">Authorization</span></span>|<span data-ttu-id="73ba6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="73ba6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73ba6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="73ba6-123">Accept</span></span>|<span data-ttu-id="73ba6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="73ba6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73ba6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73ba6-125">Request body</span></span>
<span data-ttu-id="73ba6-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „userInstallStateSummary“ an.</span><span class="sxs-lookup"><span data-stu-id="73ba6-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="73ba6-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „userInstallStateSummary“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="73ba6-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="73ba6-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73ba6-128">Property</span></span>|<span data-ttu-id="73ba6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="73ba6-129">Type</span></span>|<span data-ttu-id="73ba6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73ba6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73ba6-131">id</span><span class="sxs-lookup"><span data-stu-id="73ba6-131">id</span></span>|<span data-ttu-id="73ba6-132">String</span><span class="sxs-lookup"><span data-stu-id="73ba6-132">String</span></span>|<span data-ttu-id="73ba6-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="73ba6-133">Key of the entity.</span></span>|
|<span data-ttu-id="73ba6-134">userName</span><span class="sxs-lookup"><span data-stu-id="73ba6-134">userName</span></span>|<span data-ttu-id="73ba6-135">String</span><span class="sxs-lookup"><span data-stu-id="73ba6-135">String</span></span>|<span data-ttu-id="73ba6-136">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="73ba6-136">User name.</span></span>|
|<span data-ttu-id="73ba6-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73ba6-137">installedDeviceCount</span></span>|<span data-ttu-id="73ba6-138">Int32</span><span class="sxs-lookup"><span data-stu-id="73ba6-138">Int32</span></span>|<span data-ttu-id="73ba6-139">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="73ba6-139">Installed Device Count.</span></span>|
|<span data-ttu-id="73ba6-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73ba6-140">failedDeviceCount</span></span>|<span data-ttu-id="73ba6-141">Int32</span><span class="sxs-lookup"><span data-stu-id="73ba6-141">Int32</span></span>|<span data-ttu-id="73ba6-142">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="73ba6-142">Failed Device Count.</span></span>|
|<span data-ttu-id="73ba6-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="73ba6-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="73ba6-144">Int32</span><span class="sxs-lookup"><span data-stu-id="73ba6-144">Int32</span></span>|<span data-ttu-id="73ba6-145">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="73ba6-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="73ba6-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="73ba6-146">Response</span></span>
<span data-ttu-id="73ba6-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="73ba6-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73ba6-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73ba6-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="73ba6-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73ba6-149">Request</span></span>
<span data-ttu-id="73ba6-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73ba6-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
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

### <a name="response"></a><span data-ttu-id="73ba6-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="73ba6-151">Response</span></span>
<span data-ttu-id="73ba6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73ba6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



