# Readme

Dear our cloud computing team, here's the specification of required API endpoints from mobile developer team.

---

## Browse Campaign

- URL

  - `/campaign`

- Method

  - `GET`

- Parameters

  - `categoryId` as int, optional. -> category
  - `q` as string, optional. -> queries/keywords

- Headers
  - Authorization: `Bearer <idToken>`

## Dashboard

- URL

  - `/dashboard`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <idToken>`

## Categories

- URL

  - `/categories`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <idToken>`

## Campaign Detail

- URL

  - `/detail`

- Method

  - `GET`

- Parameters

  - `id` as int

- Headers
  - Authorization: `Bearer <idToken>`

## Task Completion Proof

- URL

  - `/proof`

- Method

  - `POST`

- Request Body

  - `taskId` as int
  - `photo` as file, optional
  - `caption` as string, optional

- Headers
  - Content-Type: `multipart/form-data`
  - Authorization: `Bearer <idToken>`

## Submit Campaign Completion

- URL

  - `/completecampaign`

- Method

  - `POST`

- Request Body

  - `campaignId ` as int

- Headers
  - Authorization: `Bearer <idToken>`

## Contributions

- URL

  - `/contributions`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <idToken>`

## Join Campaign

- URL

  - `/joincampaign`

- Method

  - `POST`

- Request Body

  - `campaignId ` as int

- Headers
  - Authorization: `Bearer <idToken>`

## Get Saved Recognisables

- URL

  - `/savedrecognisables`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <idToken>`

## Save Recognisable

- URL

  - `/saverecognisable`

- Method

  - `POST`

- Request Body

  - `label` as string
  - `confidencePercent` as int (0-100)

- Headers
  - Authorization: `Bearer <idToken>`
