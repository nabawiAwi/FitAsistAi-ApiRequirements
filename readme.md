# Readme
---

## Regiter

- URL

  - `/user/register`

- Method

  - `POST`

- Request Body

  - `username` as string, required.
  - `email` as string, required.
  - `password` as string, required.

- Samples
  - [Sample 1](https://github.com/nabawiAwi/FitAsistAi-ApiRequirements/blob/master/response_samples/register.json)


## Login

- URL

  - `/user/login`

- Method

  - `POST`

- Request Body
  
  - `email` as string, required.
  - 'password' as string, required.
  
- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20dashboard.json)

## Information

- URL

  - `/app/information`

- Method

  - `POST`
 
- Request Body
  
  - `age` as number.
  - `weight` as number.
  - `height` as number.
  - `gender` as string.

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20categories.json)

## Profile 

- URL

  - `/app/profile`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/get%20detail%20campaign.json)


## Result  

- URL

  - `/app/result`

- Method

  - `POST`

- Request Body

  - `type` as string
  - `times` as number
  - `reps` as number
  - `menit` as number

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20mission%20completion%20proof.json)


## History

- URL

  - `/app/history`

- Method

  - `GET`

- Headers

  - Authorization: `Bearer <idToken>`

- Samples
  - [Sample 1](https://github.com/EcoSenseID/EcoSense-ApiRequirements/blob/master/response_samples/post%20submit%20campaign%20completion.json)
