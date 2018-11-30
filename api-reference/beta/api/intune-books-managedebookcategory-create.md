---
title: Erstellen von managedEBookCategory
description: Erstellen eines neuen ManagedEBookCategory-Objekts.
ms.openlocfilehash: 8750e8c520e3a48b2da93d05b9f701c7760b6a15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064521"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="50325-103">Erstellen von managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="50325-103">Create managedEBookCategory</span></span>

> <span data-ttu-id="50325-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="50325-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50325-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50325-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50325-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="50325-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50325-107">Erstellen eines neuen [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="50325-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50325-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50325-108">Prerequisites</span></span>
<span data-ttu-id="50325-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50325-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50325-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50325-111">Permission type</span></span>|<span data-ttu-id="50325-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50325-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50325-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50325-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50325-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50325-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50325-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50325-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50325-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50325-116">Not supported.</span></span>|
|<span data-ttu-id="50325-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50325-117">Application</span></span>|<span data-ttu-id="50325-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50325-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50325-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50325-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="50325-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50325-120">Request headers</span></span>
|<span data-ttu-id="50325-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="50325-121">Header</span></span>|<span data-ttu-id="50325-122">Wert</span><span class="sxs-lookup"><span data-stu-id="50325-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50325-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50325-123">Authorization</span></span>|<span data-ttu-id="50325-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50325-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50325-125">Accept</span><span class="sxs-lookup"><span data-stu-id="50325-125">Accept</span></span>|<span data-ttu-id="50325-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50325-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50325-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50325-127">Request body</span></span>
<span data-ttu-id="50325-128">Geben Sie im Textkörper Anforderung für das Objekt ManagedEBookCategory eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="50325-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="50325-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ManagedEBookCategory erstellen.</span><span class="sxs-lookup"><span data-stu-id="50325-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="50325-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50325-130">Property</span></span>|<span data-ttu-id="50325-131">Typ</span><span class="sxs-lookup"><span data-stu-id="50325-131">Type</span></span>|<span data-ttu-id="50325-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50325-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50325-133">id</span><span class="sxs-lookup"><span data-stu-id="50325-133">id</span></span>|<span data-ttu-id="50325-134">String</span><span class="sxs-lookup"><span data-stu-id="50325-134">String</span></span>|<span data-ttu-id="50325-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="50325-135">The key of the entity.</span></span>|
|<span data-ttu-id="50325-136">displayName</span><span class="sxs-lookup"><span data-stu-id="50325-136">displayName</span></span>|<span data-ttu-id="50325-137">String</span><span class="sxs-lookup"><span data-stu-id="50325-137">String</span></span>|<span data-ttu-id="50325-138">Der Name der Kategorie eBook.</span><span class="sxs-lookup"><span data-stu-id="50325-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="50325-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50325-139">lastModifiedDateTime</span></span>|<span data-ttu-id="50325-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50325-140">DateTimeOffset</span></span>|<span data-ttu-id="50325-141">Datum und Uhrzeit der letzten Änderung der ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="50325-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="50325-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="50325-142">Response</span></span>
<span data-ttu-id="50325-143">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="50325-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50325-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50325-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="50325-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50325-145">Request</span></span>
<span data-ttu-id="50325-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50325-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="50325-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="50325-147">Response</span></span>
<span data-ttu-id="50325-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50325-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





