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
  - Authorization: `Bearer <idToken>`, optional

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
  - Authorization: `Bearer <idToken>`, optional

## Campaign Detail

- URL

  - `/detail`

- Method

  - `GET`

- Parameters

  - `id` as int

- Headers
  - Authorization: `Bearer <idToken>`, optional

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

## Get Stories

- URL

  - `/stories`

- Parameters

  - `page` as int, optional
  - `size` as int, optional

- Method

  - `GET`

- Headers
  - (optional) Authorization: `Bearer <token>`

## Get Story Replies

- URL

  - `/replies`

- Parameters

  - `storyId` as int
  - `page` as int, optional
  - `size` as int, optional

- Method

  - `GET`

- Headers
  - (optional) Authorization: `Bearer <token>`

## Get Story Supporters

- URL

  - `/supporters`

- Parameters

  - `storyId` as int
  - `page` as int, optional
  - `size` as int, optional

- Method

  - `GET`

- Headers
  - (optional) Authorization: `Bearer <token>`

## Post a New Story

- URL

  - `/poststory`

- Method

  - `POST`

- Headers

  - Content-Type: multipart/form-data
  - Authorization: `Bearer <token>`

- Request Body

  - `sharedCampaignId` as int, optional
  - `caption` as string
  - `attachedPhoto` as file, optional

## Post a New Reply

- URL

  - `/postreply`

- Method

  - `POST`

- Request Body

  - `storyId` as int
  - `caption` as string
  - `attachedPhoto` as file, optional

- Headers

  - Content-Type: multipart/form-data
  - Authorization: `Bearer <idToken>`

## Support a Story

- URL

  - `/supportstory`

- Method

  - `POST`

- Request Body

  - `storyId` as int

- Headers
  - Authorization: `Bearer <idToken>`

## Support a Reply

- URL

  - `/supportreply`

- Method

  - `POST`

- Request Body

  - `replyId` as int

- Headers
  - Authorization: `Bearer <idToken>`

## Reward Homepage

- URL

  - `/rewardhome`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <idToken>`, optional

## Reward List

- URL

  - `/rewards`

- Method

  - `GET`

- Parameters

  - `rewardCategory` as string

- Headers
  - Authorization: `Bearer <idToken>`, optional

## My Reward List

- URL

  - `/myrewards`

- Method

  - `GET`

- Headers
  - Authorization: `Bearer <idToken>`

## Reward Detail

- URL

  - `/rewarddetail`

- Method

  - `GET`

- Parameters

  - `rewardId` as int

- Headers
  - Authorization: `Bearer <idToken>`, optional

## My Reward Detail

- URL

  - `/myrewarddetail`

- Method

  - `GET`

- Parameters

  - `rewardId` as int

- Headers
  - Authorization: `Bearer <idToken>`, optional


## Redeem Reward

- URL

  - `/redeemreward`

- Method

  - `POST`

- Request Body

  - `rewardId` as int
  - `rewardCategory` as string

- Headers
  - Authorization: `Bearer <idToken>`

## Request Reward

- URL

  - `/requestreward`

- Method

  - `POST`

- Request Body

  - `rewardId ` as int
  - `email ` as string
  - `walletType ` as string
  - `walletNumber ` as string

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
