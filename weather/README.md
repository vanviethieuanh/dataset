# Vietnam weather dataset

Dataset record from **1st Jan 2009** to **Jun 18th 2021** of 40 province or city in Vietnam:

> Bac Lieu, Ho Chi Minh City, Tam Ky, Ben Tre, Hoa Binh, Tan An, Bien Hoa, Hong Gai, Thai Nguyen, Buon Me Thuot, Hue, Thanh Hoa, Ca Mau, Long Xuyen, Tra Vinh, Cam Pha, My Tho, Tuy Hoa, Cam Ranh, Nam Dinh, Uong Bi, Can Tho, Nha Trang, Viet Tri, Chau Doc, Phan Rang, Vinh, Da Lat, Phan Thiet, Vinh Long, Ha Noi, Play Cu, Vung Tau, Hai Duong, Qui Nhon, Yen Bai, Hai Phong, Rach Gia, Hanoi, Soc Trang

## Files

| Filename    | Records | Descriptions |
| ----------- | ------- | ------------ |
| weather.csv | 181960  | None         |

## Fields


| Column key | Description                  | Note       |
| ---------- | ---------------------------- | ---------- |
| province   | Province where data recorded | dd/mm/yyyy |
| max        | Max tempeture of the day     | Celcius    |
| min        | Min tempeture of the day     | Celcius    |
| wind       | Wind speed (mod)             | km/h       |
| wind_d     | Wind Direction               |            |
| rain       | Amount of rain               | mm         |
| humidi     | Humidity                     | %          |
| cloud      | Cloud                        | %          |
| pressure   |                              | Bar        |
| date       | Date record                  | yyyy-mm-dd |

## Samples

| province | max  | min  | wind | wind_d | rain | humidi | cloud | pressure | date       |
| -------- | ---- | ---- | ---- | ------ | ---- | ------ | ----- | -------- | ---------- |
| Bac Lieu | 27   | 22   | 17   | NNE    | 6.9  | 90     | 71    | 1010     | 2009-01-01 |
| Bac Lieu | 31   | 25   | 20   | ENE    | 0.0  | 64     | 24    | 1010     | 2010-01-01 |
| Bac Lieu | 29   | 24   | 14   | E      | 0.0  | 75     | 45    | 1008     | 2011-01-01 |
| Bac Lieu | 30   | 24   | 30   | E      | 0.0  | 79     | 52    | 1012     | 2012-01-01 |
| Bac Lieu | 31   | 25   | 20   | ENE    | 0.0  | 70     | 24    | 1010     | 2013-01-01 |

...

### Wind Directions

| direction       | sign | degree | from   | to     |
| --------------- | ---- | ------ | ------ | ------ |
| North           | N    | 0      | 348.75 | 11.25  |
| North-Northeast | NNE  | 22.5   | 11.25  | 33.75  |
| Northeast       | NE   | 45     | 33.75  | 56.25  |
| East-Northeast  | ENE  | 67.5   | 56.25  | 78.75  |
| East            | E    | 90     | 78.75  | 101.25 |
| East-Southeast  | ESE  | 112.5  | 101.25 | 123.75 |
| Southeast       | SE   | 135    | 123.75 | 146.25 |
| South-Southeast | SSE  | 157.5  | 146.25 | 168.75 |
| South           | S    | 180    | 168.75 | 191.25 |
| South-Southwest | SSW  | 202.5  | 191.25 | 213.75 |
| Southwest       | SW   | 225    | 213.75 | 236.25 |
| West-Southwest  | WSW  | 247.5  | 236.25 | 258.75 |
| West            | W    | 270    | 258.75 | 281.25 |
| West-Northwest  | WNW  | 292.5  | 281.25 | 303.75 |
| Northwest       | NW   | 315    | 303.75 | 326.25 |
| North-Northwest | NNW  | 337.5  | 326.25 | 348.75 |