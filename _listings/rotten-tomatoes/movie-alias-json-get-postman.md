{
  "info": {
    "name": "Rotten Tomatoes Get Movie Alias",
    "_postman_id": "33488117-a565-4e71-b6d0-fff066e46f39",
    "description": "Get movie alias.json.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "d8834158-f7aa-4ead-be96-a6328d0168ae",
          "name": "getLists.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fab1403d-2e79-49dd-bc0b-7014979ac769"
            }
          ]
        },
        {
          "id": "ec811fca-7dcc-43a1-afc1-092a1021f4cb",
          "name": "getListsDvds.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a88018b-dfbf-43c1-b06b-2500c7677399"
            }
          ]
        },
        {
          "id": "f28c7a86-9697-40c0-9490-8ed43f79871f",
          "name": "getListsDvdsCurrentReleases.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/current_releases.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds current releases.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2490ea0-caad-4d7f-bc83-0ff54ba7646f"
            }
          ]
        },
        {
          "id": "f2448a87-8f58-41b1-bcbe-d6fbca545662",
          "name": "getListsDvdsNewReleases.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/new_releases.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds new releases.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2a74f10-4338-4d24-b35e-29bef78d142e"
            }
          ]
        },
        {
          "id": "ad34240a-de8d-4eda-9faf-57f9d03ed89d",
          "name": "getListsDvdsTopRentals.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/top_rentals.json?country=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds top rentals.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27a80375-c32b-4717-9d59-d528489bad8e"
            }
          ]
        },
        {
          "id": "58a60aad-7506-43b1-84de-f3727c4d7412",
          "name": "getListsDvdsUpcoming.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/upcoming.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds upcoming.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09e537f5-9658-428b-9138-39e6c9d60e62"
            }
          ]
        },
        {
          "id": "9600aacc-f7d1-4f56-9aa5-7c5770a730ce",
          "name": "getListsMovies.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/movies.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists movies.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "771e46bc-480e-46f7-b3a6-39fb0663212d"
            }
          ]
        },
        {
          "id": "816d2506-cb63-43d1-92df-32c368a77bfb",
          "name": "getListsMoviesBoxOffice.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/movies/box_office.json?country=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists movies box office.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e71167b-4410-4536-ab9a-5ae86797c47d"
            }
          ]
        },
        {
          "id": "fd61b340-bafa-4b50-a85d-3686322d47ee",
          "name": "getListsMoviesInTheaters.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/movies/in_theaters.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists movies in theaters.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac92dec2-b03e-4ff3-a666-3892047677a6"
            }
          ]
        },
        {
          "id": "abf530ca-5e62-4717-bee3-96a580f2ddbc",
          "name": "getListsMoviesOpening.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/movies/opening.json?country=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists movies opening.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a23fc09-afcc-458e-b417-68a3033dadd6"
            }
          ]
        },
        {
          "id": "5cfd4f27-c57b-4cae-8093-088aaf7cfc0f",
          "name": "getListsMoviesUpcoming.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/movies/upcoming.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists movies upcoming.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa5ed17b-2e27-4367-852e-33ba7ca3d831"
            }
          ]
        }
      ]
    },
    {
      "name": "Movie",
      "item": [
        {
          "id": "74b52b3e-452d-45b2-97a8-65df2bb77f2a",
          "name": "getMovieAlias.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/movie_alias.json?id=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get movie alias.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3d10957-77f3-4212-9dd8-df9cce35175f"
            }
          ]
        }
      ]
    }
  ]
}