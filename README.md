## GraphQL API 
#### Movie API example based on GraphQL [Node.js + Express.js].

```js
type Movie {
    id: String!,
    name: String,
    gender: String,
    ranking: Int,
    year_release: Int,
    cover: String
}

type Query {
    GetMovie: [Movie!]!
    GetMovieByID(_id: String): Movie
}

type Mutation {
    CreateMovie(
        name: String,
        gender: String,
        ranking: Int,
        year_release: Int,
        cover: String
    ): Movie!
    DeleteMovie(_id: String): Movie!
    UpdateMovie(
        _id: String,
        name: String,
        gender: String,
        ranking: Int,
        year_release: Int,
        cover: String
    ): Movie!
}
```
