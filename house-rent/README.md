# House Rent Data

This is collection of posts for house rent in Vietnam. For images data of posts, please contact `vanviethieuanh@gmail.com`:

Data set contains:

| Filename | Records | Descriptions          |
| -------- | ------- | --------------------- |
| hcm.json | 5000    | Ho Chi Minh City data |

## Data and handling

This is the sample of data.

```json
[
    ...
    {
        "title": "Cho thu\u00ea ph\u00f2ng tr\u1ecd 38m2 - Kh\u00f4ng chung ch\u1ee7",
        "price": 4.2,
        "published": "23/09/2019",
        "acreage": 38.0,
        "address": "161/10 \u0110\u01b0\u1eddng \u00c2u C\u01a1, Ph\u01b0\u1eddng 14, Qu\u1eadn 11, H\u1ed3 Ch\u00ed Minh"
    },
    ...
]
```

Natively, `python (3.8)` will decode this string to:

```python
[
    ...
    {
        'title': 'Cho thuê phòng trọ 38m2 - Không chung chủ',
        'price': 4.2, 
        'published': '23/09/2019', 
        'acreage': 38.0, 
        'address': '161/10 Đường Âu Cơ, Phường 14, Quận 11, Hồ Chí Minh'
    },
    ...
]
```



### Data fields

| Column name  | Column key | Description             | Note                                                       |
| ------------ | ---------- | ----------------------- | ---------------------------------------------------------- |
| Title        | title      | Title of the post       |                                                            |
| Published in | published  | Date published          | dd/mm/yyyy                                                 |
| Address      | address    | Address in detail       |                                                            |
| Acreage      | acreage    | Acreage in square meter |                                                            |
| Price        | price      | Price in millions VND   | If price is `-1`, it mean the owner want to disscuss more. |

