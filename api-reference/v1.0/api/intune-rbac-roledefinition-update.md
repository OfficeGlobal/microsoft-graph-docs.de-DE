---
title: roleDefinition aktualisieren
description: Aktualisiert die Eigenschaften von Objekten des Typs roleDefinition.
ms.openlocfilehash: 2ceb1024b45efdf47deabac3c90fe923638f42d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017109"
---
# <a name="update-roledefinition"></a><span data-ttu-id="c19e9-103">roleDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c19e9-103">Update roleDefinition</span></span>

> <span data-ttu-id="c19e9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c19e9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c19e9-105">Aktualisiert die Eigenschaften von Objekten des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="c19e9-105">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c19e9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c19e9-106">Prerequisites</span></span>
<span data-ttu-id="c19e9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c19e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c19e9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c19e9-109">Permission type</span></span>|<span data-ttu-id="c19e9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c19e9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c19e9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c19e9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c19e9-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c19e9-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c19e9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c19e9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c19e9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c19e9-114">Not supported.</span></span>|
|<span data-ttu-id="c19e9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c19e9-115">Application</span></span>|<span data-ttu-id="c19e9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c19e9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c19e9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c19e9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="c19e9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c19e9-118">Request headers</span></span>
|<span data-ttu-id="c19e9-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c19e9-119">Header</span></span>|<span data-ttu-id="c19e9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c19e9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c19e9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c19e9-121">Authorization</span></span>|<span data-ttu-id="c19e9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c19e9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c19e9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c19e9-123">Accept</span></span>|<span data-ttu-id="c19e9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c19e9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c19e9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c19e9-125">Request body</span></span>
<span data-ttu-id="c19e9-126">Geben Sie im Anforderungstext eine JSON-Darstellung des Objekts des Typs [roleDefinition](../resources/intune-rbac-roledefinition.md) an.</span><span class="sxs-lookup"><span data-stu-id="c19e9-126">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="c19e9-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [roleDefinition](../resources/intune-rbac-roledefinition.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c19e9-127">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="c19e9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c19e9-128">Property</span></span>|<span data-ttu-id="c19e9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c19e9-129">Type</span></span>|<span data-ttu-id="c19e9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c19e9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c19e9-131">id</span><span class="sxs-lookup"><span data-stu-id="c19e9-131">id</span></span>|<span data-ttu-id="c19e9-132">String</span><span class="sxs-lookup"><span data-stu-id="c19e9-132">String</span></span>|<span data-ttu-id="c19e9-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c19e9-133">Key of the entity.</span></span> <span data-ttu-id="c19e9-134">Er ist schreibgeschützt und wird automatisch generiert.</span><span class="sxs-lookup"><span data-stu-id="c19e9-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c19e9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c19e9-135">displayName</span></span>|<span data-ttu-id="c19e9-136">String</span><span class="sxs-lookup"><span data-stu-id="c19e9-136">String</span></span>|<span data-ttu-id="c19e9-137">Anzeigename der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="c19e9-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="c19e9-138">description</span><span class="sxs-lookup"><span data-stu-id="c19e9-138">description</span></span>|<span data-ttu-id="c19e9-139">String</span><span class="sxs-lookup"><span data-stu-id="c19e9-139">String</span></span>|<span data-ttu-id="c19e9-140">Beschreibung der Rollendefinition</span><span class="sxs-lookup"><span data-stu-id="c19e9-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="c19e9-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="c19e9-141">rolePermissions</span></span>|<span data-ttu-id="c19e9-142">Sammlung von Objekten des Typs [rolePermission](../resources/intune-rbac-rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="c19e9-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="c19e9-143">Liste der Rollenberechtigungen, die dieser Rolle erteilt wurden.</span><span class="sxs-lookup"><span data-stu-id="c19e9-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="c19e9-144">Diese müssen mit dem Wert für „actionName“ übereinstimmen, der als Teil von „rolePermission“ festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="c19e9-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="c19e9-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="c19e9-145">isBuiltIn</span></span>|<span data-ttu-id="c19e9-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c19e9-146">Boolean</span></span>|<span data-ttu-id="c19e9-147">Rollentyp.</span><span class="sxs-lookup"><span data-stu-id="c19e9-147">Type of Role.</span></span> <span data-ttu-id="c19e9-148">Ist auf „True“ gesetzt, wenn es sich um eine integrierte Rolle handelt, und auf „False“, wenn es sich um eine benutzerdefinierte Rollendefinition handelt.</span><span class="sxs-lookup"><span data-stu-id="c19e9-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="c19e9-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="c19e9-149">Response</span></span>
<span data-ttu-id="c19e9-150">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [roleDefinition](../resources/intune-rbac-roledefinition.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c19e9-150">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c19e9-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c19e9-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="c19e9-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c19e9-152">Request</span></span>
<span data-ttu-id="c19e9-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c19e9-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="c19e9-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="c19e9-154">Response</span></span>
<span data-ttu-id="c19e9-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c19e9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



