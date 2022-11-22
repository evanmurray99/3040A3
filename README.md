# Title of API
`This text goes over the topic of API` <br>
Consectetur adipiscing elit.
Fusce non lacus blandit, porta nunc nec, malesuada leo. Quisque eleifend
augue arcu, non malesuada ipsum rhoncus id. In blandit sapien eu nisl
pellentesque, gravida condimentum neque bibendum.

---

# Resource(s)
`
The resource description is brief (1-3 sentences) and usually starts with
a verb. Resources usually have various endpoints to access the resource and
multiple methods for each endpoint. On the same page, you usually have a
general resource described along with a number of endpoints for accessing
the resource, also described. Also, ensure that the description is
formatted as JSON`<br>

Consectetur adipiscing elit.
Fusce non lacus blandit, porta nunc nec, malesuada leo. Quisque eleifend
augue arcu, non malesuada ipsum rhoncus id. In blandit sapien eu nisl
pellentesque, gravida condimentum neque bibendum. Mauris ut orci ultricies,
consequat neque ut, dignissim ex. Duis vitae sem efficitur, blandit arcu nec,
vestibulum nulla. Morbi sed sem ligula.

# Resource(s) Endpoints

`
Typically, an API will have a number of endpoints grouped under the
same resource. In this case, you describe both the general resource
and the individual endpoints.
`<br>



| Endpoint Type | Endpoint | Description |
| ----------- | ----------- | ----------- |
| GET | /resource_base/{data_type}/ | Get basic resource |
| GET | /resource_base/{section}/{data_type} | Get basic resource from specific section |

## GET /resource_base/{data_type}/?access_token=ACCESS-TOKEN
` https://api.ourapi.com/v1/resource_base/{data_type}/?access_token=ACCESS-TOKEN `<br><br>
Get basic resource.

### Requirements
**ACCESS_TOKEN**
> A valid access token.

### Parameters
**data_type**
The required data type to be returned.

Choose from either:
- type1
- type2

### Example: Request and Response
```
https://api.ourapi.com/v1/resource_base/type1/?access_token=ACCESS-TOKEN
```
<br>

```
[
    {
      "employee": {
      "name": "Stewart",
      "ID": 3.14159
      }
    },
    {
      "employee": {
      "name": "Jerome",
      "ID": 2.71828
      }
    }
]
```



## GET /resource_base/{section}/{data_type}/?access_token=ACCESS-TOKEN
` https://api.ourapi.com/v1/resource_base/{section}/{data_type}/?access_token=ACCESS-TOKEN `<br><br>
Get basic resource from a specific section.

**ACCESS_TOKEN**
> A valid access token.

### Parameters
**section**
The section of data to be queried.

Choose from either:
- section1
- section2

**data_type**
The required data type to be returned.

Choose from either:
- type1
- type2

### Example: Request and Response
```
https://api.ourapi.com/v1/resource_base/section1/type1/?access_token=ACCESS-TOKEN
```
<br>

```
[
    {
      "employee": {
      "name": "Stewart",
      "ID": 3.14159
      }
    },
    {
      "employee": {
      "name": "Jerome",
      "ID": 2.71828
      }
    }
]
```



---
