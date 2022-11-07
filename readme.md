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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20browse%20campaign.json)

## Dashboard

- URL

  - `/dashboard`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20dashboard.json)

## Categories

- URL

  - `/categories`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <idToken>`, optional

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20categories.json)

## Campaign Detail

- URL

  - `/detail`

- Method

  - `GET`

- Parameters

  - `id` as int

- Headers

  - Authorization: `Bearer <idToken>`, optional

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20detail%20campaign%201.json)
  - [Sample 2](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20detail%20campaign%202.json)

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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20task%20completion%20proof.json)

## Submit Campaign Completion

- URL

  - `/completecampaign`

- Method

  - `POST`

- Request Body

  - `campaignId ` as int

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20submit%20campaign%20completion.json)

## Contributions

- URL

  - `/contributions`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20contributions.json)

## Join Campaign

- URL

  - `/joincampaign`

- Method

  - `POST`

- Request Body

  - `campaignId ` as int

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20join%20campaign.json)

## Get Saved Recognisables

- URL

  - `/savedrecognisables`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20saved%20recognisables.json)

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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20save%20recognisable.json)

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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20stories.json)

## Get Story Detail

- URL

  - `/storydetail`

- Parameters

  - `id` as int

- Method

  - `GET`

- Headers

  - (optional) Authorization: `Bearer <token>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20story%20detail.json)

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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20story%20replies.json)

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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20story%20supporters.json)

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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20a%20new%20story.json)

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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20a%20new%20reply.json)

## Support a Story

- URL

  - `/supportstory`

- Method

  - `POST`

- Request Body

  - `storyId` as int

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20support%20a%20story.json)

## Unsupport a Story

- URL

  - `/unsupportstory`

- Method

  - `POST`

- Request Body

  - `storyId` as int

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20unsupport%20a%20story.json)

## Support a Reply

- URL

  - `/supportreply`

- Method

  - `POST`

- Request Body

  - `replyId` as int

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20support%20a%20reply.json)

## Unsupport a Reply

- URL

  - `/unsupportreply`

- Method

  - `POST`

- Request Body

  - `replyId` as int

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20unsupport%20a%20reply.json)

## Reward Homepage

- URL

  - `/rewardhome`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <idToken>`, optional

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20reward%20homepage.json)

## Reward List

- URL

  - `/rewards`

- Method

  - `GET`

- Parameters

  - `categoryId` as int

- Headers

  - Authorization: `Bearer <idToken>`, optional

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20reward%20list.json)

## My Reward List

- URL

  - `/myrewards`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20my%20reward%20list.json)

## Reward Detail

- URL

  - `/rewarddetail`

- Method

  - `GET`

- Parameters

  - `rewardId` as int

- Headers

  - Authorization: `Bearer <idToken>`, optional

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20reward%20detail.json)

## My Reward Detail

- URL

  - `/myrewarddetail`

- Method

  - `GET`

- Parameters

  - `claimId` as int

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20my%20reward%20detail.json)

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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20redeem%20reward.json)

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

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20request%20reward.json)

## Use Reward

- URL

  - `/usereward`

- Method

  - `POST`

- Request Body

  - `claimId ` as int

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20use%20reward.json)

## Get Profile

- URL

  - `/profile`

- Method

  - `GET`

- Parameters

  - `userId` as int, optional

- Headers

  - Authorization: `Bearer <idToken>`, optional

- Samples
  - [Self profile](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20profile.json)
  - [Other's profile](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20others%20profile.json)

## Get Stories History

- URL

  - `/storieshistory`

- Method

  - `GET`

- Parameters

  - `userId` as int, optional

- Headers

  - Authorization: `Bearer <idToken>`, optional

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20stories%20history.json)

## Get Campaigns History

- URL

  - `/campaignshistory`

- Method

  - `GET`

- Parameters

  - `userId` as int, optional

- Headers

  - Authorization: `Bearer <idToken>`, optional

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20campaigns%20history.json)

## Get Notifications

- URL

  - `/notifications`

- Method

  - `GET`

- Parameters

  - `language` as string ('id' OR 'en')

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20notifications.json)
