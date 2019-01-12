---
title: Aktualisieren von „userInstallStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 67e1ced8cf96c4b3ac51eee314cfd092dcaca8da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972691"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="06632-103">Aktualisieren von „userInstallStateSummary“</span><span class="sxs-lookup"><span data-stu-id="06632-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="06632-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="06632-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06632-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="06632-105">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06632-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="06632-106">Prerequisites</span></span>
<span data-ttu-id="06632-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06632-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06632-109">Permission type</span></span>|<span data-ttu-id="06632-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06632-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06632-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06632-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06632-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06632-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06632-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06632-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06632-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06632-114">Not supported.</span></span>|
|<span data-ttu-id="06632-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06632-115">Application</span></span>|<span data-ttu-id="06632-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06632-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06632-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06632-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="06632-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06632-118">Request headers</span></span>
|<span data-ttu-id="06632-119">Header</span><span class="sxs-lookup"><span data-stu-id="06632-119">Header</span></span>|<span data-ttu-id="06632-120">Wert</span><span class="sxs-lookup"><span data-stu-id="06632-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06632-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06632-121">Authorization</span></span>|<span data-ttu-id="06632-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="06632-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06632-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="06632-123">Accept</span></span>|<span data-ttu-id="06632-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06632-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06632-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06632-125">Request body</span></span>
<span data-ttu-id="06632-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="06632-126">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="06632-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="06632-127">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="06632-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06632-128">Property</span></span>|<span data-ttu-id="06632-129">Typ</span><span class="sxs-lookup"><span data-stu-id="06632-129">Type</span></span>|<span data-ttu-id="06632-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06632-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06632-131">id</span><span class="sxs-lookup"><span data-stu-id="06632-131">id</span></span>|<span data-ttu-id="06632-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06632-132">String</span></span>|<span data-ttu-id="06632-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="06632-133">Key of the entity.</span></span>|
|<span data-ttu-id="06632-134">userName</span><span class="sxs-lookup"><span data-stu-id="06632-134">userName</span></span>|<span data-ttu-id="06632-135">String</span><span class="sxs-lookup"><span data-stu-id="06632-135">String</span></span>|<span data-ttu-id="06632-136">Name des Benutzers</span><span class="sxs-lookup"><span data-stu-id="06632-136">User name.</span></span>|
|<span data-ttu-id="06632-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06632-137">installedDeviceCount</span></span>|<span data-ttu-id="06632-138">Int32</span><span class="sxs-lookup"><span data-stu-id="06632-138">Int32</span></span>|<span data-ttu-id="06632-139">Anzahl der installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="06632-139">Installed Device Count.</span></span>|
|<span data-ttu-id="06632-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06632-140">failedDeviceCount</span></span>|<span data-ttu-id="06632-141">Int32</span><span class="sxs-lookup"><span data-stu-id="06632-141">Int32</span></span>|<span data-ttu-id="06632-142">Anzahl der fehlgeschlagenen Geräte</span><span class="sxs-lookup"><span data-stu-id="06632-142">Failed Device Count.</span></span>|
|<span data-ttu-id="06632-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="06632-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="06632-144">Int32</span><span class="sxs-lookup"><span data-stu-id="06632-144">Int32</span></span>|<span data-ttu-id="06632-145">Anzahl der nicht installierten Geräte</span><span class="sxs-lookup"><span data-stu-id="06632-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="06632-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="06632-146">Response</span></span>
<span data-ttu-id="06632-147">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="06632-147">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06632-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06632-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="06632-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06632-149">Request</span></span>
<span data-ttu-id="06632-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06632-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="06632-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="06632-151">Response</span></span>
<span data-ttu-id="06632-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06632-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



