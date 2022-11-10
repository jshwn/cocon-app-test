# cocon-app-test

### Lint

- [lefthook](https://github.com/evilmartians/lefthook)

```bash
> lefthook install
```

### Design

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2F1VXFX2ehPKRawc56eIVwIs%2FCOCON-APP%3Fnode-id%3D0%253A1" allowfullscreen></iframe>

[링크](https://www.figma.com/file/1VXFX2ehPKRawc56eIVwIs/COCON-APP?node-id=0%3A1)

## API

### Request

```http
// 아우터
GET https://cf-api-c.brandi.me/v1/web/categories/218/products?offset=0&limit=100&type=all&order=popular
Authorization: 3b17176f2eb5fdffb9bafdcc3e4bc192b013813caddccd0aad20c23ed272f076_1423639497

GET https://cf-api-c.brandi.me/v1/web/categories/373/products?offset=0&limit=100&type=all&order=popular
Authorization: 3b17176f2eb5fdffb9bafdcc3e4bc192b013813caddccd0aad20c23ed272f076_1423639497
```

### Response

```http
{
    "meta": {
        "advertisement_info": {
            "is_category_ad": true,
            "is_today_ad": false,
            "is_home_ad": true,
            "is_search_ad": true,
            "is_special_exhibition_ad": false,
            "is_best_ad": false,
            "is_product_detail_ad": true,
            "is_order_complete_ad": true,
            "is_cart_ad": true
        },
        "code": 200,
        "count": 100
    },
    "data": [
        {
            "id": "82469399",
            "image_thumbnail_url": "https://image.brandi.me/cproduct/2022/10/14/SB000000000075118717_1665717802_image1_S.webp",
            "image_medium_url": "https://image.brandi.me/cproduct/2022/10/14/SB000000000075118717_1665717802_image1_S.webp",
            "image_url": "https://image.brandi.me/cproduct/2022/10/14/SB000000000075118717_1665717802_image1_M.webp",
            "web_image_thumbnail_url": "https://image.brandi.me/cproduct/2022/10/14/SB000000000075118717_1665717798_image1_S.jpeg",
            "web_image_medium_url": "https://image.brandi.me/cproduct/2022/10/14/SB000000000075118717_1665717798_image1_S.jpeg",
            "web_image_url": "https://image.brandi.me/cproduct/2022/10/14/SB000000000075118717_1665717798_image1_M.jpeg",
            "name": "폭스 퍼 구스 다운 자켓 [아이보리]",
            "price": 179000,
            "sale_price": 179000,
            "sale_percent": 0,
            "is_sell": true,
            "is_special_price": false,
            "is_new": false,
            "is_free_delivery": true,
            "is_heart_delivery": false,
            "is_today_delivery": false,
            "bookmark_count": 12,
            "seller": {
                "id": "33554",
                "name": "레프트",
                "en_name": "left",
                "image_url": "https://image.brandi.me/seller/leftseoul_profile_1616561984.jpg",
                "text": "레프트(LEFT)는 우리가 살아가는 현재와 과거에서 영감을 받아 어디에서든 입을 수 있는 옷을 추구합니다.",
                "is_brandstore": true,
                "is_partner": false
            },
            "root_category_no": "217",
            "root_category_name": "브랜드"
        },
        ...
    ]
}
```
