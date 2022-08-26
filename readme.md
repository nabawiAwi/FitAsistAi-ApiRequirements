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

# Get Stories

- URL

  - `/stories`

- Parameters

  - `page` as int, optional
  - `size` as int, optional

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <token>`

# Get Story Comments

- URL

  - `/comments`

- Parameters

  - `storyId` as int

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <token>`

# Post a New Story

- URL

  - `/poststory`

- Method
  - `POST`

Headers

- Content-Type: multipart/form-data
- Authorization: `Bearer <token>`

Request Body

- `caption` as string
- `photo` as file, optional, must be a valid image file, max size 1MB

# Post a Comment

- URL

  - `/postcomment`

- Method

  - `POST`

- Request Body

  - `storyId` as int
  - `content` as string

- Headers
  - Authorization: `Bearer <idToken>`

# Like a Story

- URL

  - `/likestory`

- Method

  - `POST`

- Request Body

  - `storyId` as int

- Headers
  - Authorization: `Bearer <idToken>`

# Like a Comment

- URL

  - `/likecomment`

- Method

  - `POST`

- Request Body

  - `commentId` as int

- Headers
  - Authorization: `Bearer <idToken>`

## Reward Homepage

- URL

  - `/rewardhome`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <idToken>`

## Reward List

- URL

  - `/rewards`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <idToken>`

## Reward Detail

- URL

  - `/rewarddetail`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <idToken>`

## Redeem Reward

- URL

  - `/redeemreward`

- Method

  - `POST`

- Request Body

  - `rewardId` as int

- Headers
  - Authorization: `Bearer <idToken>`

## Use Reward

- URL

  - `/usereward`

- Method

  - `POST`

- Request Body

  - `rewardId ` as int

- Headers
  - Authorization: `Bearer <idToken>`
