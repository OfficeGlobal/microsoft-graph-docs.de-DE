# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="0228c-101">Aktualisieren einer app in einem team</span><span class="sxs-lookup"><span data-stu-id="0228c-101">Upgrade an app in a team</span></span>



<span data-ttu-id="0228c-102">Führt ein Upgrade einer [app-Installation](../resources/teamsappinstallation.md) in einem [Team](../resources/team.md) auf die neueste Version der app.</span><span class="sxs-lookup"><span data-stu-id="0228c-102">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="0228c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0228c-103">Permissions</span></span>

<span data-ttu-id="0228c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0228c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0228c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0228c-106">Permission type</span></span>      | <span data-ttu-id="0228c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0228c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0228c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0228c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0228c-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0228c-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0228c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0228c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0228c-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0228c-111">Not supported.</span></span>    |
|<span data-ttu-id="0228c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0228c-112">Application</span></span> | <span data-ttu-id="0228c-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0228c-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0228c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0228c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="0228c-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0228c-115">Request headers</span></span>
| <span data-ttu-id="0228c-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0228c-116">Header</span></span>       | <span data-ttu-id="0228c-117">Wert</span><span class="sxs-lookup"><span data-stu-id="0228c-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0228c-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="0228c-118">Authorization</span></span>  | <span data-ttu-id="0228c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0228c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0228c-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0228c-121">Request body</span></span>
<span data-ttu-id="0228c-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0228c-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0228c-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="0228c-123">Response</span></span>

<span data-ttu-id="0228c-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0228c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0228c-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0228c-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="0228c-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0228c-127">Request</span></span>
<span data-ttu-id="0228c-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0228c-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="0228c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="0228c-129">Response</span></span>
<span data-ttu-id="0228c-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0228c-130">The following is an example of the response.</span></span> 

><span data-ttu-id="0228c-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0228c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
