# Taxonomy

## Get all taxonomies

```shell
curl -X "GET" "https://dev2-web.hollar.com/api/taxonomies" \
	-H "Content-Type: application/json" \
	-H "Accept: application/json"
```

```javascript
jQuery.ajax({
    url: "https://dev2-web.hollar.com/api/taxonomies",
    type: "GET",
    headers: {
        "Content-Type": "application/json",
        "Accept": "application/json",
    },
})
```

```java
Content content = Request.Get("https://dev2-web.hollar.com/api/taxonomies")

.addHeader("Content-Type", "application/json")
.addHeader("Accept", "application/json")

.execute().returnContent();
}
```

```swift
let headers = [
    "Content-Type":"application/json",
    "Accept":"application/json",
]

Alamofire.request(.GET, "https://dev2-web.hollar.com/api/taxonomies", headers: headers)
    .validate(statusCode: 200..<300)
    .responseJSON { response in
      // ...
    }
}
```

> JSON Response

```json
{
  "taxonomies": [
    {
      "id": 1,
      "name": "Category",
      "root": {
        "id": 1,
        "name": "Category",
        "pretty_name": "Category",
        "permalink": "category",
        "parent_id": null,
        "taxonomy_id": 1,
        "taxons": [
          {
            "id": 2,
            "name": "Apparel & Accessories",
            "pretty_name": "Category -> Apparel & Accessories",
            "permalink": "apparel-accessories",
            "parent_id": 1,
            "taxonomy_id": 1,
            "taxons": [
              ...
            ],
            "published": true,
            "image": "https://dyryekj877zmm.cloudfront.net/dev2/spree/taxon_images/424/normal/007609-01.jpg?1454530028",
            "width": 520,
            "height": 520
          }
        ]
      }
    }
  ],
  "count": 1,
  "current_page": 1,
  "pages": 1
}
```

<aside class="notice">
This request does not require a spree token.
</aside>

Returns all the published taxonomies along with it's root taxon and taxon children.

## Get a taxon

# Taxons

## Get all taxons

## Get a taxon
