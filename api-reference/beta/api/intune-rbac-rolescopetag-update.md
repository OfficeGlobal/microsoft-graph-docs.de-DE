---
title: RoleScopeTag aktualisieren
description: Aktualisieren Sie die Eigenschaften eines RoleScopeTag-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bece75c05fa65a2c5def34ec1644a7375711ab97
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808134"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="74f31-103">RoleScopeTag aktualisieren</span><span class="sxs-lookup"><span data-stu-id="74f31-103">Update roleScopeTag</span></span>

> <span data-ttu-id="74f31-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="74f31-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74f31-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="74f31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74f31-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="74f31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74f31-107">Aktualisieren Sie die Eigenschaften eines [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="74f31-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="74f31-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="74f31-108">Prerequisites</span></span>
<span data-ttu-id="74f31-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74f31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74f31-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="74f31-111">Permission type</span></span>|<span data-ttu-id="74f31-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="74f31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74f31-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="74f31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74f31-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74f31-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="74f31-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="74f31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74f31-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74f31-116">Not supported.</span></span>|
|<span data-ttu-id="74f31-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="74f31-117">Application</span></span>|<span data-ttu-id="74f31-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="74f31-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74f31-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="74f31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="74f31-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="74f31-120">Request headers</span></span>
|<span data-ttu-id="74f31-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="74f31-121">Header</span></span>|<span data-ttu-id="74f31-122">Wert</span><span class="sxs-lookup"><span data-stu-id="74f31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74f31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74f31-123">Authorization</span></span>|<span data-ttu-id="74f31-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="74f31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74f31-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="74f31-125">Accept</span></span>|<span data-ttu-id="74f31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74f31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74f31-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="74f31-127">Request body</span></span>
<span data-ttu-id="74f31-128">Geben Sie im Textkörper Anforderung für das Objekt [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="74f31-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="74f31-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [RoleScopeTag](../resources/intune-rbac-rolescopetag.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="74f31-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="74f31-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74f31-130">Property</span></span>|<span data-ttu-id="74f31-131">Typ</span><span class="sxs-lookup"><span data-stu-id="74f31-131">Type</span></span>|<span data-ttu-id="74f31-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74f31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f31-133">id</span><span class="sxs-lookup"><span data-stu-id="74f31-133">id</span></span>|<span data-ttu-id="74f31-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="74f31-134">String</span></span>|<span data-ttu-id="74f31-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="74f31-135">Key of the entity.</span></span> <span data-ttu-id="74f31-136">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="74f31-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="74f31-137">displayName</span><span class="sxs-lookup"><span data-stu-id="74f31-137">displayName</span></span>|<span data-ttu-id="74f31-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="74f31-138">String</span></span>|<span data-ttu-id="74f31-139">Das Display oder den Anzeigenamen des Tags Bereich Rolle.</span><span class="sxs-lookup"><span data-stu-id="74f31-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="74f31-140">description</span><span class="sxs-lookup"><span data-stu-id="74f31-140">description</span></span>|<span data-ttu-id="74f31-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="74f31-141">String</span></span>|<span data-ttu-id="74f31-142">Beschreibung des Tags Bereich Rolle.</span><span class="sxs-lookup"><span data-stu-id="74f31-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="74f31-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="74f31-143">Response</span></span>
<span data-ttu-id="74f31-144">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [RoleScopeTag](../resources/intune-rbac-rolescopetag.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="74f31-144">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74f31-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="74f31-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="74f31-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="74f31-146">Request</span></span>
<span data-ttu-id="74f31-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="74f31-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="74f31-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="74f31-148">Response</span></span>
<span data-ttu-id="74f31-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="74f31-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





