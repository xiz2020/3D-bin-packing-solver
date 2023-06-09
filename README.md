**#Description:**

The 3D Bin Packing Problem (3D-BPP) is one of the most frequent problems in warehousing and logistics. Its solution is filling a container (a box or pallet) with items as closely to each other as possible to minimize the number of required containers.

![image](https://external-preview.redd.it/oWu9Rd_ykjnEAfbnDQZkc8aq3eNpgvJdZ2rtExtMTNw.png?auto=webp&s=c87aef08f0e2e1536cb4c28a5c420ae5cf5f2d51)

**API**

https://rapidapi.com/zilinskivan/api/3d-bin-packing-problem/

**Body request example:**

<pre>
{
  "boxes": [
    {
      "name": "Box 1",
      "width": 15,
      "height": 15,
      "length": 15,
      "weight": 30
    }
  ],
  "products": [
    {
      "name": "BLACK-TSHIRT-XSMALL",
      "width": 15,
      "height": 15,
      "length": 3,
      "weight": 0.15,
      "qty": 18
    }
  ]
}
</pre>

**Rsponse (Solution):**

<pre>
{
  "s": 1,
  "data": [
    {
      "name": "Box 1",
      "length": 15,
      "width": 15,
      "height": 15,
      "weight_used": 0.75,
      "items_in_box": 5,
      "products": [
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        }
      ]
    },
    {
      "name": "Box 1",
      "length": 15,
      "width": 15,
      "height": 15,
      "weight_used": 0.75,
      "items_in_box": 5,
      "products": [
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        }
      ]
    },
    {
      "name": "Box 1",
      "length": 15,
      "width": 15,
      "height": 15,
      "weight_used": 0.6,
      "items_in_box": 4,
      "products": [
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        }
      ]
    },
    {
      "name": "Box 1",
      "length": 15,
      "width": 15,
      "height": 15,
      "weight_used": 0.6,
      "items_in_box": 4,
      "products": [
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        },
        {
          "name": "BLACK-TSHIRT-XSMALL",
          "length": 3,
          "width": 15,
          "height": 15,
          "weight": 0.15
        }
      ]
    }
  ]
}
</pre>

**Code Samples:**

**CURL**

<pre>
curl --request POST \
  --url https://3d-bin-packing-problem.p.rapidapi.com/ \
  --header 'X-RapidAPI-Host: 3d-bin-packing-problem.p.rapidapi.com' \
  --header 'X-RapidAPI-Key: Your Key' \
  --data '{"boxes":[{"name":"Box 1","width":15,"height":15,"length":15,"weight":30}],"products":[{"name":"BLACK-TSHIRT-XSMALL","width":15,"height":15,"length":3,"weight":0.15,"qty":18}]}'
</pre>

**Javascript:**

<pre>
const settings = {
  "async": true,
  "crossDomain": true,
  "url": "https://3d-bin-packing-problem.p.rapidapi.com/",
  "method": "POST",
  "headers": {
    "X-RapidAPI-Key": "Your Key",
    "X-RapidAPI-Host": "3d-bin-packing-problem.p.rapidapi.com"
  },
  "processData": false,
  "data": {
    "boxes": [
      {
        "name": "Box 1",
        "width": 15,
        "height": 15,
        "length": 15,
        "weight": 30
      }
    ],
    "products": [
      {
        "name": "BLACK-TSHIRT-XSMALL",
        "width": 15,
        "height": 15,
        "length": 3,
        "weight": 0.15,
        "qty": 18
      }
    ]
  }
};

$.ajax(settings).done(function (response) {
  console.log(response);
});
</pre>

**NodeJS:**

<pre>
import axios from "axios";

const options = {
  method: 'POST',
  url: 'https://3d-bin-packing-problem.p.rapidapi.com/',
  headers: {
    'X-RapidAPI-Key': 'Your Key',
    'X-RapidAPI-Host': '3d-bin-packing-problem.p.rapidapi.com'
  },
  data: '{"boxes":[{"name":"Box 1","width":15,"height":15,"length":15,"weight":30}],"products":[{"name":"BLACK-TSHIRT-XSMALL","width":15,"height":15,"length":3,"weight":0.15,"qty":18}]}'
};

axios.request(options).then(function (response) {
  console.log(response.data);
}).catch(function (error) {
  console.error(error);
});
</pre>

**PHP**

<pre>
<?php

$client = new http\Client;
$request = new http\Client\Request;

$body = new http\Message\Body;
$body->append('{"boxes":[{"name":"Box 1","width":15,"height":15,"length":15,"weight":30}],"products":[{"name":"BLACK-TSHIRT-XSMALL","width":15,"height":15,"length":3,"weight":0.15,"qty":18}]}');

$request->setRequestUrl('https://3d-bin-packing-problem.p.rapidapi.com/');
$request->setRequestMethod('POST');
$request->setBody($body);

$request->setHeaders([
  'X-RapidAPI-Key' => 'Your Key',
  'X-RapidAPI-Host' => '3d-bin-packing-problem.p.rapidapi.com'
]);

$client->enqueue($request)->send();
$response = $client->getResponse();

echo $response->getBody();
</pre>
