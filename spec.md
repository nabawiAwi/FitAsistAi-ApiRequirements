## Browse Campaign

- URL

  - `/campaign`

- Method

  - `GET`

- Parameters

  1.  `cat` as string, optional. -> category
  2.  `q` as string, optional. -> queries/keywords

- Headers
  - Authorization: `Bearer <token>`

## Dashboard

- URL

  - `/dashboard`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <token>`

## Categories

- URL

  - `/categories`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <token>`

## Campaign Detail

- URL

  - `/detail`

- Method

  - `GET`

- Parameters

  - `id` as int

- Headers
  - Authorization: `Bearer <token>`

## Task Completion Proof

- URL

  - `/proof`

- Method

  - `POST`

- Request Body

  - `photo` as file

- Headers
  - Content-Type: `multipart/form-data`
  - Authorization: `Bearer <token>`

## Submit Campaign Completion

- URL

  - `/completecampaign`

- Method

  - `POST`

- Request Body

  - `campaignId ` as int

- Headers
  - Authorization: `Bearer <token>`

## Profile

- URL

  - `/profile`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <token>`

## Join Campaign

- URL

  - `/joincampaign`

- Method

  - `POST`

- Request Body

  - `campaignId ` as int

- Headers
  - Authorization: `Bearer <token>`